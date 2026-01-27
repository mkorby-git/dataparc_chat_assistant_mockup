# dataPARC Assistant Interactive Mockup
## Agent-Driven Mini User Guide (v3.0)

**Version:** 3.0 (Agent-Driven)  
**Last Updated:** January 2026

---

## What Is This?

The **dataPARC Assistant Agent-Driven Mockup** is an interactive HTML prototype demonstrating an AI-powered chat assistant for industrial process control. It showcases how specialized AI agents can help plant operators, process engineers, and maintenance technicians gain insights from process data.

**Key Concept:** Users select specialized agents that control the assistant's behavior and expertise area - similar to consulting different subject matter experts.

**Important:** This is a static prototype with pre-scripted responses. It demonstrates visual design and interaction patterns but does not connect to real dataPARC data or use live AI.

---

## Five Specialized Agents

Each agent is a specialist with unique capabilities:

**⚙️ dataPARC Configuration Helper** (Default)
- Helps with dataPARC setup, trending configuration, and alarm rules
- Shows "Common Tasks" panel with setup suggestions
- Best for: Learning dataPARC features, configuring new tags

**🤖 General Process Assistant**
- All-purpose monitoring and general insights
- Best for: Routine monitoring, general questions

**🏭 Kamyr Digester Specialist**
- Deep expertise in digester operations, H-factor, kappa number, liquor circulation
- Provides specialized digester performance analysis
- Best for: Pulp mill operators working with Kamyr digesters

**🔴 Critical Alert Monitor**
- Real-time alarm monitoring with structured alert presentation
- Shows red alert banner with trajectory predictions
- Best for: Emergency response, critical process deviations

**🔍 Root Cause Analyst**
- Incident investigation with timeline visualization
- Structured analysis with contributing factors and confidence levels
- Best for: Post-incident analysis, understanding what went wrong

---

## Quick Start Guide

### Opening the Mockup
1. Open `dataparc-assistant-agent-driven_3-0.html` in any modern browser (Chrome, Edge, Firefox, Safari)
2. The interface displays in two panes:
   - **Left:** Simulated dataPARC trend chart area with chart selector
   - **Right:** AI Assistant chat panel (420px wide)

### Selecting an Agent
1. Look at the **Active Agent** dropdown in the assistant header (blue banner)
2. Click the dropdown to see all 5 agents
3. Select an agent - the interface automatically adapts:
   - Context bar shows the agent's specialty
   - Opening message changes to match agent's expertise
   - Chart area indicator shows active agent name

### Interacting with Agents

**dataPARC Configuration Helper:**
- Click any task in the "🎯 Common Tasks" panel
- Tasks populate the input field
- Examples: "Help me set up trending for new tags", "Create alarm rules"

**Other Agents (General, Kamyr):**
- See "💡 Suggestions based on current view" with quick action buttons
- Type your own questions in the input field
- Try: "What caused the spike?" or "Analyze anomalies"

**Critical Alert Monitor:**
- Shows red alert banner automatically
- Displays current value, limit, rate of change, and trajectory
- Action buttons: Investigate, Acknowledge, View History

**Root Cause Analyst:**
- Pre-loaded with sample incident analysis
- Shows timeline, contributing factors, recommendations
- Expandable sections for detailed methodology

### Key Features
- **Auto-scroll:** Conversation automatically scrolls to show latest messages
- **Context Bar:** Shows active agent specialty (changes when you switch agents)
- **Thinking Indicator:** Three pulsing dots when assistant is "analyzing"
- **Agent-specific behavior:** Each agent has unique personality and opening messages

---

## Quick Reference

### Agent Selection Guide

| When to Use | Select This Agent |
|-------------|-------------------|
| Learning dataPARC, setting up tags/alarms | ⚙️ Configuration Helper |
| General monitoring, routine questions | 🤖 General Process Assistant |
| Digester performance, H-factor, kappa | 🏭 Kamyr Digester Specialist |
| Critical alarms, emergency response | 🔴 Critical Alert Monitor |
| Understanding past incidents, RCA | 🔍 Root Cause Analyst |

### Technical Overview

**Browser Compatibility:**
- ✅ Chrome/Edge (recommended)
- ✅ Firefox
- ✅ Safari
- ❌ Internet Explorer (not supported)

**File Structure:**
- Single self-contained HTML file (~65KB, ~1520 lines)
- Inline CSS styles and React components
- No external dependencies except CDN-hosted React 18
- No network requests after initial load

**What This Mockup Does NOT Include:**
- Real AI/LLM integration
- Actual dataPARC data connections
- User authentication or security
- Data persistence (refreshing resets state)
- Responsive mobile design (optimized for desktop 1920x1080+)
- Accessibility features (screen readers, keyboard navigation)

---

## Key Differences from Version 1.x

**What's New:**
- Agent-driven architecture (agents control behavior, not separate "modes")
- Five specialized agents with unique personalities
- Context bar shows active agent specialty
- Common Tasks panel for Configuration Helper agent
- Auto-scroll in conversation area
- Cleaner header (removed redundant information)

**What's Removed:**
- "Demo Mode" dropdown (agents now control behavior)
- "Currently viewing" trend information (redundant with main display)
- Separate mode state management

---

## Next Steps for Production

To convert this mockup to a production system:

1. **Backend Integration:** Connect to dataPARC APIs for real-time data
2. **AI Integration:** Implement LLM service with agent-specific prompts and context
3. **Data Analysis Engine:** Build statistical analysis, correlation detection, predictive algorithms
4. **User Authentication:** Role-based access control, agent permissions
5. **Agent Builder:** Allow users to create custom agents for their specific processes
6. **Responsive Design:** Adapt layout for tablets and mobile devices
7. **Accessibility:** ARIA labels, keyboard navigation, screen reader support
8. **Real-time Updates:** WebSocket connections for live data streaming
9. **Testing:** Unit tests, integration tests, user acceptance testing with operators

---

**END OF GUIDE**

*This guide describes version 3.0 of the dataPARC Assistant Agent-Driven Mockup*
