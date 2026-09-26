# 🎮 TOON Playground

An interactive web playground for exploring **TOON (Token-Oriented Object Notation)** - a token-efficient data format optimized for Large Language Models.

## 🌟 Features

- **Live Format Comparison**: Convert JSON to TOON, YAML instantly and see side-by-side comparisons
- **Token Analysis**: Real-time token counting showing exact savings (30-60% reduction vs JSON)
- **OpenAI Integration**: Test your data with OpenAI's API in different formats
- **Pre-built Examples**: Load ready-to-use examples demonstrating various data structures
- **Beautiful UI**: Modern, responsive design with Poppins and Inter fonts
- **Educational**: Learn how TOON works with visual examples and explanations

## 🚀 Quick Start

### Prerequisites

- Python 3.10 or higher
- [uv](https://github.com/astral-sh/uv) (Python package manager)
- OpenAI API key (optional, for LLM testing)

### Installation

1. **Install dependencies with uv:**

```bash
# Install uv if you haven't already
curl -LsSf https://astral.sh/uv/install.sh | sh

# Install project dependencies
uv sync
```

2. **Set up your OpenAI API key (optional):**

Edit the `.env` file and add your OpenAI API key:

```env
OPENAI_API_KEY=sk-your-actual-api-key-here
```

Get your API key from: https://platform.openai.com/api-keys

3. **Run the playground:**

```bash
# Using uv
uv run uvicorn app:app --reload

# Or with Python directly
python -m uvicorn app:app --reload
```

4. **Open in browser:**

Navigate to: http://localhost:8000

## 📚 What is TOON?

TOON (Token-Oriented Object Notation) is a compact, human-readable data format designed specifically for LLM prompts. It provides:

### Key Benefits

- **📊 40-60% Token Reduction**: Dramatically reduce token usage compared to JSON
- **🔁 JSON Compatible**: Lossless conversion to/from JSON
- **📐 Tabular Arrays**: CSV-style format for uniform data
- **🎯 LLM-Optimized**: Clearer structure improves model comprehension
- **💰 Cost Savings**: Lower token count = lower API costs

### Example Transformation

**JSON (verbose):**
```json
{
  "users": [
    {"id": 1, "name": "Alice", "role": "admin"},
    {"id": 2, "name": "Bob", "role": "user"}
  ]
}
```

**TOON (compact):**
```toon
users[2]{id,name,role}:
  1,Alice,admin
  2,Bob,user
```

**Result**: ~40% fewer tokens! 🎉

## 🎯 Use Cases

### Perfect For:
- ✅ Tabular data (database results, CSV-like data)
- ✅ Arrays of uniform objects
- ✅ Analytics and metrics
- ✅ Product catalogs
- ✅ RAG search results

### Not Ideal For:
- ❌ Deeply nested structures
- ❌ Highly irregular data
- ❌ Very small datasets (overhead not worth it)

## 🏗️ Architecture

### Backend (FastAPI + Python)
- **`app.py`**: Main FastAPI application with REST API endpoints
- **`toon_encoder.py`**: TOON encoding/decoding implementation
- **API Endpoints**:
  - `POST /api/convert`: Convert JSON to all formats
  - `POST /api/llm-test`: Test with OpenAI API
  - `GET /api/examples`: Get example datasets
  - `GET /api/health`: Health check

### Frontend (Vanilla JS + Modern CSS)
- **`static/index.html`**: Main playground interface
- **`static/style.css`**: Modern, responsive styling with CSS variables
- **`static/script.js`**: Interactive functionality and API integration

### Features:
- Real-time format conversion
- Token count visualization
- Side-by-side format comparison
- OpenAI API integration
- Copy-to-clipboard functionality
- Toast notifications
- Responsive design

## 📊 Token Savings Examples

### Employee Records (100 entries)
- JSON: 6,360 tokens
- TOON: 2,518 tokens
- **Savings: 60%** 🎉

### Analytics Data (60 days)
- JSON: 22,250 tokens
- TOON: 9,120 tokens
- **Savings: 59%** 🎉

### GitHub Repositories (100 repos)
- JSON: 15,145 tokens
- TOON: 8,745 tokens
- **Savings: 42%** 🎉

## 🔧 API Usage

### Convert JSON to TOON

```bash
curl -X POST http://localhost:8000/api/convert \
  -H "Content-Type: application/json" \
  -d '{"json_data": "{\"users\": [{\"id\": 1, \"name\": \"Alice\"}]}"}'
```

### Test with OpenAI

```bash
curl -X POST http://localhost:8000/api/llm-test \
  -H "Content-Type: application/json" \
  -d '{
    "format": "toon",
    "data": "users[1]{id,name}:\n  1,Alice",
    "prompt": "List all users"
  }'
```

## 📖 Learn More

- **TOON Specification**: https://github.com/toon-format/spec
- **Official Documentation**: https://toonformat.dev
- **TypeScript Implementation**: https://github.com/toon-format/toon

## 📝 License

Proprietary — all rights reserved. This code is published for viewing and evaluation only; no use, copying, modification, redistribution, commercial use, or use as AI/ML training data without written permission. See [LICENSE](LICENSE). Commercial licensing: aianytime07@gmail.com · sonu@aianytime.net.

---

**Built by AI Anytime with ❤️ for the AI community**

Reduce tokens, save costs, improve performance! 🚀
