# dataPARC Assistant Interactive Mockup
## Mini User Guide

**Version:** 1.0  
**Last Updated:** January 2026

---

## What Is This?

The **dataPARC Assistant Enhanced Mockup** is an interactive HTML prototype demonstrating an AI-powered chat assistant for industrial process control. It shows how an intelligent assistant could help plant operators, process engineers, and maintenance technicians gain insights from process data.

**Key Concept:** The assistant's personality is modeled after an experienced shift supervisor with 15+ years of process industry experience - professional, precise, and proactive.

**Important:** This is a static prototype with pre-scripted responses. It demonstrates visual design and interaction patterns but does not connect to real dataPARC data or use live AI.

---

## Core Design Principles

### 1. Context Awareness
The assistant adapts through four operational modes:
- **Normal Operations:** Proactive monitoring with contextual suggestions
- **Critical Alert:** Urgent but calm presentation of safety-critical information
- **Root Cause Analysis:** Structured, evidence-based incident investigation
- **Idle Mode:** Helpful suggestions for common tasks

### 2. Information Hierarchy
Critical information first, with progressive disclosure:
1. Direct answers and key metrics (always visible)
2. Supporting data and correlations (immediately visible)
3. Reasoning and methodology (expandable sections)
4. Data sources and metadata (collapsible sections)

### 3. Visual Alert Severity
- **Critical Alerts:** Red gradient banner with animation
- **Normal Messages:** Purple accent with subtle styling
- **User Messages:** Blue background for clear identification
- **System Context:** Light blue informational banner

### 4. Data Transparency
All insights include:
- Specific data source tags (e.g., TR_102_TEMP, FC_201_RATE)
- Expandable "Show reasoning" sections
- Clear timestamps and time ranges
- Explicit confidence levels (e.g., "High Confidence")

### 5. Respectful Collaboration
- Uses "I recommend" rather than "You must"
- Presents options without forcing choices
- Acknowledges user expertise through professional tone
- Provides actionable information without condescension

---

## Quick Start Guide

### Opening the Mockup
1. Open `dataparc-assistant-mockup-enhanced_1-0.html` in any modern web browser (Chrome, Edge, Firefox, Safari)
2. The interface displays in two panes:
   - **Left:** Simulated dataPARC trend chart area
   - **Right:** AI Assistant chat panel (420px wide)

### Exploring the Four Modes

Use the **Demo Mode** dropdown (top-right corner) to switch between scenarios:

**Mode 1: Normal Operations**
- Shows proactive monitoring during routine operations
- Assistant identifies temperature excursions pattern
- Context bar shows currently viewed trend
- Try clicking the suggested quick actions

**Mode 2: Critical Alert**
- Demonstrates urgent notification during safety-critical event
- Red animated banner with structured alert details
- Shows current value (158 PSI), limit (150 PSI), rate of change (+2 PSI/minute)
- Includes trajectory prediction: "165 PSI in 3.5 minutes without intervention"

**Mode 3: Root Cause Analysis**
- Structured investigation of a past incident
- Timeline visualization (13:55 through 14:45)
- Contributing factors with confidence badges
- Recommended preventive actions

**Mode 4: Idle / Smart Suggestions**
- Common task suggestions when no active analysis
- Click any suggestion to populate the input field
- Examples: "Show me tags trending outside normal ranges," "Check H-factor, cooking temps"

### Interactive Elements

**Typing Questions:**
1. Click in the text input field (bottom of assistant panel)
2. Type a question (try: "What caused the spike?" or "Analyze anomalies")
3. Press Enter or click "Send ➤"
4. Watch the thinking animation (3 pulsing dots)
5. Response appears after 2 seconds

**Note:** Questions containing "spike" or "cause" trigger detailed analysis responses.

**Expandable Sections:**
- Click "▶ Show reasoning" to see analytical methodology
- Click "▶ Data Sources Used" to see tag names and time ranges
- Arrow changes from ▶ (collapsed) to ▼ (expanded)

**Visual Indicators:**
- **Mode Indicator (bottom-left):** Purple badge showing current mode
- **Context Bar (below header):** Blue panel showing what data is being analyzed
- **Confidence Badges:** Green badges showing certainty level
- **Message Icons:** 🤖 for Assistant, 👤 for User

---

## Technical Overview

### Browser Compatibility
✅ Chrome/Edge (recommended)  
✅ Firefox  
✅ Safari  
❌ Internet Explorer (not supported)

### File Structure
- Single self-contained HTML file (~60KB, ~1360 lines)
- Inline CSS styles and React components
- No external dependencies except CDN-hosted libraries (React 18)
- No network requests after initial load

### What This Mockup Does NOT Include
- Real AI/LLM integration
- Actual dataPARC data connections
- User authentication or security
- Data persistence (refreshing resets state)
- Responsive mobile design (optimized for desktop 1920x1080+)
- Accessibility features (screen readers, keyboard navigation)

---

## Quick Reference

### Mode Comparison

| Mode | Color | Purpose | Key Feature |
|------|-------|---------|-------------|
| Normal Operations | Purple | Proactive monitoring | Contextual suggestions |
| Critical Alert | Red | Emergency notification | Structured alert data |
| Root Cause Analysis | Purple | Post-incident investigation | Timeline visualization |
| Idle | Gray | Task discovery | Common task suggestions |

### Design Color Palette

- **Primary (Assistant):** #7C3AED (Purple 600)
- **Secondary (Data):** #2E5C8A (Blue 700)
- **Critical (Alerts):** #DC2626 (Red 600)
- **Context (Info):** #0369a1 (Sky 700)
- **Background:** #f5f7fa (Gray 50)
- **Text:** #374151 (Gray 700)

### Next Steps for Production

To convert this mockup to a production system:
1. **Backend Integration:** Connect to dataPARC APIs for real-time data
2. **AI Integration:** Implement LLM service for natural language understanding
3. **Data Analysis Engine:** Build statistical analysis and correlation detection
4. **User Authentication:** Implement role-based access control
5. **Responsive Design:** Adapt layout for tablets and mobile
6. **Accessibility:** Add ARIA labels, keyboard navigation, screen reader support
7. **Testing:** Unit tests, integration tests, user acceptance testing

---

**END OF GUIDE**

*This guide describes version 1.0 of the dataPARC Assistant Enhanced Mockup (dataparc-assistant-mockup-enhanced_1-0.html)*
