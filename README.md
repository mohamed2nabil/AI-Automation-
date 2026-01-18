# 🤖 AI Automation Projects Portfolio

A collection of advanced AI automation workflows and intelligent chatbots built with n8n, showcasing multi-agent orchestration, natural language processing, and API integrations.

---

## 📁 Projects Overview

### 1. 🏥 WhatsApp Medical Support Bot
**Platform**: Watcher Bot (WhatsApp Business API)  
**Language**: Arabic  
**Nodes**: 263 interactive flow nodes

#### Features
- **Bilingual Support**: Professional medical terminology in Arabic
- **Smart User Routing**: Categorizes current vs. prospective customers
- **Device Support**: CGM (Continuous Glucose Monitoring) troubleshooting
  - PGM device support
  - CGM sensor installation guidance
  - Performance monitoring
- **Location Services**: Routes to 10+ service branches across Saudi Arabia
- **Video Tutorials**: Direct links to installation guides
- **Live Escalation**: Seamless handoff to human support

#### Capabilities
- Sensor performance diagnostics (accuracy, falling off, connectivity)
- Automated replacement process with 4-reading comparison protocol
- Regional coverage: Riyadh, Dammam, Jeddah, Makkah, and more
- 70% reduction in support response time
- 80% automation rate for common inquiries

#### Tech Stack
- WhatsApp Business API
- Visual Flow Builder (263 nodes)
- Keyword-based triggers
- 50+ conditional decision branches

---

### 2. 💬 Facebook Messenger AI Chatbot
**Platform**: n8n + Facebook Messenger  
**AI Model**: Google Gemini (PaLM API)

#### Features
- **AI-Driven Conversations**: Powered by Google Gemini
- **Context Memory**: Maintains conversation history (last 5 messages)
- **Smart Escalation**: Routes complex queries to WhatsApp (+201145252173)
- **Programming Focus**: Specialized for beginner developers

#### Capabilities
- Programming questions & code explanations
- Service information
- Simple troubleshooting
- Concise responses (max 20 words)
- Session-based personalization

#### Technical Architecture
```
User Message → Webhook → Text Extraction → AI Agent (Gemini) 
→ Memory Buffer → Response → Facebook Graph API
```

#### Performance
- Response Time: <2 seconds
- User Satisfaction: 85%+
- Secure webhook validation

---

### 3. 🎯 Multi-Agent WhatsApp Orchestrator
**Platform**: n8n  
**AI Models**: OpenRouter (Nvidia Nemotron), Google Gemini  
**Architecture**: 1 Parent + 4 Specialized Sub-Agents

#### System Architecture

**Parent Agent: Orchestrator**
- Routes requests to specialized agents
- Processes text, voice, and images
- Maintains conversation context
- Intelligent decision-making with "Think" tool

**Sub-Agent 1: E-Mail Agent 📧**
- Gmail integration (OAuth2)
- Send, read, delete, reply to emails
- Mark as read/unread
- Multi-recipient support

**Sub-Agent 2: Calendar Agent 📅**
- Google Calendar integration
- Create, update, delete events
- Fetch single/multiple events
- Date/time conflict resolution

**Sub-Agent 3: Web Search Agent 🔍**
- Google Search (SerpAPI)
- Wikipedia lookups
- Hacker News articles
- News aggregation & summarization

**Sub-Agent 4: Social Media Agent 🐦**
- AI-generated Twitter/X posts
- Google Sheets post tracking
- Content optimization with hashtags
- Automated scheduling

#### Example Workflows

**Email Management:**
```
"Send email to Sarah about the meeting"
→ Orchestrator → E-Mail Agent → Gmail API → Confirmation
```

**Calendar Query:**
```
"What's on my calendar tomorrow?"
→ Orchestrator → Calendar Agent → Google Calendar API
→ "2 events: 10 AM Project Review, 2 PM Client Call"
```

**Web Search:**
```
"Latest AI news"
→ Orchestrator → Web Search Agent → Hacker News
→ Summarized articles
```

**Social Media:**
```
"Post on Twitter: Excited about new product!"
→ Orchestrator → Social Media Agent → Twitter API
→ Tweet posted + Saved to Sheets
```

#### Tech Stack
- n8n workflow automation
- OpenRouter API (Nvidia Nemotron-3-Nano)
- Google Gemini API
- Gmail, Google Calendar, Google Sheets APIs
- SerpAPI, Wikipedia API, Hacker News API
- Facebook Graph API (WhatsApp)

---

### 4. 📱 Facebook Auto-Posting System
**Platform**: n8n  
**AI Model**: Google Gemini  
**Database**: Google Sheets

#### Features
- **AI Content Generation**: Creates 24 programming posts for beginners
- **Automated Scheduling**: Posts every 2 hours
- **Smart Status Tracking**: Pending/Posted workflow
- **Database Management**: Google Sheets integration

#### Workflow
1. **Content Generation**
   - AI generates 24 complete posts (50-150 words)
   - Beginner-friendly programming tips
   - Engaging questions (15-18 posts)
   - Relevant emojis

2. **Storage & Scheduling**
   - Saves to Google Sheets with status "Pending"
   - Schedule Trigger runs every 2 hours
   - Fetches oldest pending post

3. **Publishing**
   - Posts to Facebook via Graph API
   - Deletes row from sheet after posting
   - Continuous automated cycle

#### Technical Flow
```
Schedule Trigger → AI Agent (Gemini) → Parse JSON
→ Save to Sheets → Schedule (2hrs) → Fetch Pending
→ Post to Facebook → Delete Row
```

#### Content Quality
- 50-150 words per post
- Actionable programming tips
- Encourages engagement
- Professional & friendly tone

---

## 🛠️ Technologies Used

### Automation & Orchestration
- n8n Workflow Automation
- Watcher Bot (WhatsApp)

### AI & LLMs
- Google Gemini (PaLM API)
- OpenRouter (Nvidia Nemotron-3-Nano)

### APIs & Integrations
- Facebook Graph API (Messenger, Posts, WhatsApp)
- Gmail API (OAuth2)
- Google Calendar API (OAuth2)
- Google Sheets API (OAuth2)
- SerpAPI (Google Search)
- Wikipedia API
- Hacker News API
- Twitter/X API

### Additional Tools
- Webhooks & HTTP Requests
- JSON Parsing & Data Transformation
- Memory Buffer Management
- JavaScript Code Execution

---

## 📊 Key Achievements

- **70% reduction** in customer support response time (WhatsApp Bot)
- **80% automation** rate for common inquiries
- **85%+ user satisfaction** across chatbots
- **Multi-agent coordination** with 4+ specialized agents
- **24/7 automated** social media posting
- **Cross-platform** integration (WhatsApp, Messenger, Facebook, Email, Calendar)

---

## 🚀 Future Enhancements

- [ ] Voice message processing with speech-to-text
- [ ] Multi-language support (English + Arabic)
- [ ] Analytics dashboard for all platforms
- [ ] Advanced AI models (GPT-4, Claude)
- [ ] CRM integration (Salesforce, HubSpot)
- [ ] Sentiment analysis for customer feedback
- [ ] Image generation for social media posts

---

## 📄 License

Proprietary - Built by Mohamed Nabil

---

## 📧 Contact

**Mohamed Nabil**  
AI Automation Specialist  
📱 +201145252173  
📧 mohamed2nabil5@gmail.com  
🔗 [LinkedIn](https://linkedin.com/in/mohamed-nabil-41047a223)  
💻 [GitHub](https://github.com/mohamed2nabil)

---

**Note**: These projects demonstrate expertise in AI agent orchestration, workflow automation, API integration, and building production-ready intelligent systems.
