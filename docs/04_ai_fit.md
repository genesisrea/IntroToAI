# AI Fit
The problem being address is a recurring workflow issue: instrument health checks are conducted manually and the review step is often missed or delayed. Because the data exist and the workflow is predictable, it is a strong candidate for automation supported by AI. 
1. Detect: Using PowerBI, the data can be file ingested and processed. The data then gets evaluated by the calculated columns for trend violations or out of control conditions. This replaces the manual step where someone has to interpret for trends or OOC events. 
2. Trigger: Once an issue is detected, PowerBI will flag it. Power Automate will then send only the data that requires a response through an automated workflow. This ensures that every flagged condition is escalated immediately and consistently. 
3. Generate: The PowerAutomate workflow leads to a generative AI prompt which then receives the data along with the instrument conditions/history and any relative context. The AI will then respond with standardize message that addresses what the condition/trend that was detected, severity, and any potential correction actions that need to be taken. This AI-generated message is automatically emailed to the lab team during a failure notification. This gives technicians immediate visibility into the issue and helps them understand what action to take. This will ensure full compliance and audit visibility.   

AI is appropriate here because: 
- The workflow is predictable and occurs at a high frequency (every week)
- That is structured and is consistent in format. 
- A process automation has no chance of forgetting for it to happen. 
- AI is only assisting with communication and explanation