# Claude Code Worklist Extraction Strategy

## Purpose
The goal is to **extract complete and accurate worklists for each position** in a company using Claude Code in a conversational style.  
This focuses solely on **what work is done by a role**, not how tasks are triggered or assigned.  

---

## Inputs

1. **Company Structure Knowledge**
   - Positions present in the company.
   - Hierarchy and reporting lines.
   - Communication patterns between positions.

2. **LLM General Knowledge**
   - Pre-existing knowledge of typical worklists for common positions.
   - Examples: Store Manager, Software Engineer, HR Manager, etc.

3. **Previous Interview Knowledge**
   - Past interviews or information about how positions function in reality.
   - Used to validate and refine extracted worklists.

---

## Outputs

- **Worklists for each position**
  - Detailed set of tasks performed by a role.
  - Organized by frequency, priority, and domain (if applicable).
- Extracted entirely through a **conversational interview** with Claude Code.
- Free from conflicts or ambiguous interpretations.

---

## Problem Statement

1. **Conversational Style**
   - Must **encourage detailed responses** about a position’s work.
   - Should avoid questions that focus on triggers, requests, or origin of tasks.
   - Conversational tone should be **neutral, open-ended, and exploratory**.
   
2. **Best Way to Extract Worklists**
   - Ask **role-centric questions** like:
     - “What are the core tasks you handle daily/weekly?”
     - “What are the key responsibilities of your position?”
     - “What outputs or deliverables do you generate?”
   - Avoid asking **who assigns the work** or **how tasks appear**.
   - Use iterative questioning:
     - Start broad → refine → validate details → capture exceptional or rare tasks.

3. **Ensuring Conflict-Free Extraction**
   - Focus on **facts, not opinions** or interpretations.
   - Cross-check with **known position responsibilities** from LLM general knowledge.
   - Use **structured follow-ups** to clarify ambiguous tasks.
   - Categorize tasks under clear headers: Daily, Weekly, Monthly, Ad-hoc.

---

## Recommended Conversational Strategy

1. **Phase 1: Role Introduction**
   - Confirm the position and scope.
   - Example:  
     ```
     Claude: Please describe the role of the Store Manager.
     ```

2. **Phase 2: Core Work Extraction**
   - Ask for main responsibilities without asking about task triggers.
   - Example:  
     ```
     Claude: What are the main work items you handle regularly?
     ```

3. **Phase 3: Detail Expansion**
   - Drill down into each reported task.
   - Example:  
     ```
     Claude: Can you explain the steps involved in managing inventory?
     ```

4. **Phase 4: Validation & Completion**
   - Review the worklist for completeness.
   - Ask if any tasks are missing or rare but important.
   - Example:  
     ```
     Claude: Are there any tasks you perform occasionally that are critical for the position?
     ```

5. **Phase 5: Structuring**
   - Organize extracted tasks into clear categories.
   - Example:  
     - **Daily Tasks**
     - **Weekly Tasks**
     - **Monthly Tasks**
     - **Ad-hoc / Exceptional Tasks**

---

## Benefits of This Approach

- Produces **accurate, role-specific worklists**.
- Minimizes **ambiguity and conflict** in responses.
- Ensures **repeatable and scalable conversational extraction** across multiple positions.

---

## Example Output Structure

```text
Position: Store Manager

Daily Tasks:
- Check and manage inventory levels.
- Supervise staff and assign daily responsibilities.
- Review sales and operational reports.

Weekly Tasks:
- Conduct staff meetings and performance reviews.
- Plan promotional activities.
- Coordinate with suppliers for restocking.

Monthly Tasks:
- Analyze sales trends and prepare monthly reports.
- Review and update operational procedures.

Ad-hoc Tasks:
- Handle customer escalations.
- Manage special events or campaigns.
