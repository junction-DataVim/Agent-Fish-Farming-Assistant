# Fish Farming Assistant Agent Documentation

## Overview
The **Fish Farming Assistant** is an AI-powered agent designed to help manage and optimize aquaculture operations. It leverages a combination of database queries and advanced AI models (such as Groq ) to provide actionable insights, monitor pond health, analyze sensor data, and alert users to potential issues.

## Key Features
- **Sensor Data Analysis:** Query and analyze real-time and historical sensor readings (temperature, pH, dissolved oxygen, turbidity, etc.).
- **Pond Status Monitoring:** Track fish growth, survival rate, and health status for each pond.
- **Alert Management:** Review and analyze alerts for critical events (e.g., disease outbreaks, low oxygen levels).
- **Comprehensive Summaries:** Generate detailed summaries for any pond, including recent alerts and available sensors.
- **AI-Powered Insights:** Use Groq or OpenAI models to answer complex questions, provide recommendations, and explain technical data in user-friendly terms.
- **Fallback to Direct Analysis:** If no API key is set, the agent can still provide full database-driven analysis and reporting.

## Usage
1. **Setup:**
   - Install required dependencies (see `requirements.txt`).
   - Ensure the fish farming database (`fish_farming_timeseries.db`) is available and populated.
   - Set your Groq or OpenAI API key as an environment variable for AI-powered features.
2. **Available Tools:**
   - `sensor_tool`: Query sensor readings.
   - `pond_tool`: Query pond status.
   - `alert_tool`: Query alerts.
   - `summary_tool`: Get pond summary.
   - `list_tool`: List all available ponds.
3. **Agent Capabilities:**
   - Ask the agent questions about pond health, water quality, recent alerts, and receive actionable recommendations.
   - Use the agent for both manual data analysis and AI-enhanced insights.

## Example Questions
- "What is the current health status of TilapiaPond_001?"
- "Show recent sensor readings for all ponds."
- "Are there any critical alerts in the last 24 hours?"
- "Recommend actions to improve survival rate."

## Notes
- The agent is extensible: you can add new tools or connect to other AI models as needed.
- If the AI API key is not set, the agent will automatically fall back to direct database analysis.

---
