# API Reference

## Import

```javascript
const chatgptPromptEngineering = require('./chatgpt-prompt-engineering');
```

## Methods

### `analyze(input, options?)`

Main analysis function.

**Parameters:**

| Parameter | Type | Required | Default | Description |
|-----------|------|----------|---------|-------------|
| `input` | `string` | Yes | - | Input data to process |
| `options.verbose` | `boolean` | No | `false` | Enable detailed output |
| `options.format` | `string` | No | `'text'` | Output format: text, json, table |
| `options.timeout` | `number` | No | `30000` | Timeout in milliseconds |

**Returns:** `Promise<Object>`

```javascript
const result = await chatgptPromptEngineering.analyze('sample input', {
    verbose: true,
    format: 'json'
});
```

### Response Format

```json
{
    "success": true,
    "data": { ... },
    "meta": {
        "processedAt": "2025-01-01T00:00:00Z",
        "duration": "15ms"
    }
}
```

### `validate(input)`

Quick validation without full processing.

**Returns:** `{ valid: boolean, errors: string[] }`

## CLI Usage

```bash
node index.js <input>
node index.js <input> --verbose
node index.js <input> --format json
```

## Error Handling

```javascript
try {
    const result = await chatgptPromptEngineering.analyze(input);
} catch (error) {
    if (error.code === 'INVALID_INPUT') {
        console.error('Invalid input:', error.message);
    } else if (error.code === 'TIMEOUT') {
        console.error('Operation timed out');
    }
}
```
