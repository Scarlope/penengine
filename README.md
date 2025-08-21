# Pen Memory Engine

> **Next-Generation Cognitive Memory System for AI Assistants**

[![License: AGPL v3](https://img.shields.io/badge/License-AGPL%20v3-red.svg)](https://www.gnu.org/licenses/agpl-3.0)
[![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/)
[![Status: Alpha](https://img.shields.io/badge/status-unrelesed-white.svg)]()

## 🧠 What is Pen Memory Engine?

Pen Memory Engine is the **first true cognitive memory architecture** for AI assistants that goes far beyond simple conversation storage. It transforms AI from "forgetful tools" into **intelligent companions** with human-like memory capabilities.

### The Problem We Solve

**Traditional AI:**
```
User: "Remember we talked about cars last week?"
AI: "I don't have access to previous conversations. Could you provide details?"
```

**Pen Memory Engine:**
```
User: "Remember we talked about cars last week?"
AI: "Yes! You were considering a Tesla Model 3 but were unsure about the budget. 
     Did you make a decision? You also wanted to research financing options."
```

## ✨ Revolutionary Features

### 🕐 **Temporal Intelligence**
- Real-time clock integration
- Event prediction and follow-ups
- Time-aware conversations
- Gap analysis ("We haven't talked in 3 days")

### 🧬 **Personality Analysis**
- Communication pattern recognition
- Behavioral analysis
- Decision-making patterns
- Learning style adaptation

### 🔮 **Proactive Interactions**
- Predicts user needs
- Remembers commitments
- Follows up on plans
- Anticipates questions

### 📚 **7-Layer Cognitive Architecture**
- **L1**: Working Memory (Active session)
- **L2**: Complete History Archive (Full conversations)
- **L2.5**: Semantic Indexing (Topic summaries)
- **L3**: Similarity Matching (Déjà vu simulation)
- **L4**: User Intelligence (Personality & preferences)
- **L6**: Temporal Tracking (Time-aware events)
- **L7**: Future Planning (Goals & reminders)


### Basic Usage

```python
from pen_memory_engine import PenMemory

# Initialize memory system
pen = PenMemory(user_id="user123")

# Get enriched context for conversation
user_message = "I want to continue learning Python"
context = pen.get_context(user_message)

# Your normal AI call with enhanced context
messages = pen.enrich_prompt(base_messages, context)
response = openai.chat.completions.create(
    model="gpt-4",
    messages=messages
)

# Store the interaction for future recall
pen.store_interaction(user_message, response.choices[0].message.content)
```

## 🏗️ Architecture Overview

```mermaid
graph TD
    A[User Input] --> B[L1: Working Memory]
    B --> C[L3: Similarity Search]
    C --> D[L2.5: Topic Indexing]
    D --> E[L2: Full Archive]
    
    B --> F[L4: User Intelligence]
    B --> G[L6: Temporal Intelligence]
    B --> H[L7: Future Planning]
    
    F --> I[Enriched Context]
    G --> I
    H --> I
    E --> I
    
    I --> J[AI Response]
    J --> K[Memory Storage]
```

## 💡 Use Cases

### 🎓 **Learning Assistant**
```
Week 1: "I'm starting to learn Python"
Week 3: "How's your Python journey going? Did you solve that for-loop 
         challenge we discussed? What topic are you working on now?"
```

### 📋 **Project Tracking**
```
Month start: "I want to build a blog with Django"
2 weeks later: "How's your blog project? You were planning to work 
              on authentication - did you get stuck there?"
```

### 💚 **Emotional Intelligence**
```
Stressful week: "This week has been overwhelming"
Next week: "How are you feeling? Last week seemed really tough - 
           are things getting better?"
```

### 🎯 **Decision Support**
```
Decision process: "I'm thinking about buying a car - Tesla vs Toyota"
1 month later: "Did you decide on the car? Last time you were weighing 
               range vs cost. What made the final decision?"
```



## 📊 Performance

### Efficiency Metrics
- **Data Compression**: 400KB stores months of conversations
- **Response Time**: 5 seconds (API) / 18 seconds (local)
- **Memory Usage**: 8GB VRAM for full local deployment
- **Cost**: ~$0.67 per 1000 messages (Together.ai)


## 🤝 Contributing

We welcome contributions! Pen Memory Engine is developed with heavy AI assistance, making it uniquely suited for AI-enhanced development workflows.

### Development Philosophy
- **AI-First Development**: Built by humans working with AI
- **Cognitive Design**: Architecture mirrors human memory systems
- **Community-Driven**: Open source with strong community focus
- **Research-Backed**: Based on cognitive science principles

### How to Contribute

1. **Fork the repository**
2. **Create a feature branch**: `git checkout -b feature/amazing-feature`
3. **Make your changes** (AI pair programming encouraged!)
4. **Test thoroughly**: `pytest tests/`
5. **Submit a pull request**

### Contribution Areas
- 🧠 **Core Memory Layers**: Optimize existing layers
- 🔍 **New Integrations**: Connect with other AI platforms  
- 👁️ **Vision Development**: Help build V1-V4 visual layers
- 🌍 **Internationalization**: Multi-language support
- 🧪 **Testing & Edge Cases**: Improve robustness

## 📄 License

This project is licensed under the **GNU Affero General Public License v3.0 (AGPL-3.0)**.

### What this means:
- ✅ **Free for personal use, education, and open source projects**
- ✅ **Modify and redistribute freely**
- ✅ **Use in academic research**
- ❌ **Commercial use requires separate licensing**
- ❌ **Cannot be used in proprietary products**
- ❌ **SaaS offerings must open source entire stack**

### Commercial Licensing
For commercial use, enterprise licensing, or SaaS offerings, please contact us for commercial licensing options.

**Why AGPL v3?**
We chose AGPL v3 to ensure that improvements to Pen Memory Engine benefit the entire community while preventing exploitation by large corporations who would use the technology without contributing back.

## 📞 Support & Community

### 🐛 **Bug Reports & Feature Requests**
- [GitHub Issues](https://github.com/Scarlope/penengine/issues)

### 💬 **Community Discussion**
- [GitHub Discussions](https://github.com/Scarlope/penengine/discussions)


### 🏢 **Enterprise & Commercial**
- Email: mirza@scarlope.com

## 🙏 Acknowledgments

This project was developed through intensive AI-human collaboration, representing a new paradigm in AI-assisted software development. Special thanks to:

- The cognitive science research community for memory architecture insights
- The open source AI community for inspiration and feedback
- Early testers and contributors who helped shape the system
- The AI models that served as development partners

---

**Built with 🧠 by humans and AI working together**

*"Transforming AI from tools that forget into companions that remember"*
