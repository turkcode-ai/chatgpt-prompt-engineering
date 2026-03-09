# Examples

## Basic Usage

### Simple Analysis

```javascript
const chatgptPromptEngineering = require('./chatgpt-prompt-engineering');

const result = chatgptPromptEngineering.analyze('Hello World');
console.log(result);
```

### With Options

```javascript
const chatgptPromptEngineering = require('./chatgpt-prompt-engineering');

const result = await chatgptPromptEngineering.analyze('sample input', {
    verbose: true,
    format: 'json'
});

console.log(JSON.stringify(result, null, 2));
```

### File Processing

```javascript
const fs = require('fs');
const chatgptPromptEngineering = require('./chatgpt-prompt-engineering');

const content = fs.readFileSync('input.txt', 'utf8');
const result = await chatgptPromptEngineering.analyze(content);
console.log(result);
```

## CLI Examples

```bash
# Basic analysis
node index.js "test input"

# Read from stdin
cat input.txt | node index.js

# JSON output
node index.js "test" --json

# Save output to file
node index.js "test" --json > output.json

# Verbose mode
node index.js "test" --verbose
```

## Express.js Integration

```javascript
const express = require('express');
const chatgptPromptEngineering = require('./chatgpt-prompt-engineering');

const app = express();
app.use(express.json());

app.post('/analyze', async (req, res) => {
    try {
        const result = await chatgptPromptEngineering.analyze(req.body.input);
        res.json({ success: true, data: result });
    } catch (error) {
        res.status(400).json({ success: false, error: error.message });
    }
});

app.listen(3000, () => console.log('Server running on port 3000'));
```

## Batch Processing

```javascript
const chatgptPromptEngineering = require('./chatgpt-prompt-engineering');

const inputs = ['input1', 'input2', 'input3'];

const results = await Promise.all(
    inputs.map(input => chatgptPromptEngineering.analyze(input))
);

results.forEach((result, i) => {
    console.log(`Result ${i + 1}:`, result.data);
});
```

---

For more examples, visit [TurkCode AI Blog](https://turkcode.net/blog).
