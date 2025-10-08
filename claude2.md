# Position-Based Worklist Extraction System

## Overview
A conversational interview framework for systematically extracting comprehensive worklists from company positions using Claude Code, leveraging organizational structure knowledge and LLM capabilities.

---

## System Inputs

### 1. **Company Structure Knowledge**
- Position hierarchy and reporting relationships
- Inter-position communication channels
- Complete inventory of existing positions
- Organizational dependencies and workflows

### 2. **LLM General Knowledge Base**
- Industry-standard responsibilities for each position
- Common tasks and workflows by role type
- Best practices and typical work patterns
- Cross-industry position benchmarks

### 3. **Historical Interview Data**
- Previously interviewed position insights
- Identified task dependencies
- Cross-functional workflow patterns
- Validated worklist components

---

## Target Output

**Comprehensive Position Worklists** containing:
- Daily, weekly, monthly, and periodic tasks
- Position-specific responsibilities
- Cross-functional dependencies
- Communication touchpoints
- Decision-making authorities
- Performance metrics and deliverables

---

## Problem Statements & Solutions

## Problem 1: Optimal Conversational Style

### Solution: Progressive Discovery Framework

#### **Recommended Style: Consultative-Narrative Approach**

**Core Principles:**
1. **Context-First**: Begin with understanding before questioning
2. **Collaborative Tone**: Partner stance rather than interrogative
3. **Adaptive Depth**: Adjust detail level based on position complexity
4. **Validation Loops**: Confirm understanding iteratively

**Conversation Structure:**

```
Phase 1: Context Setting (10%)
├─ Acknowledge position role in organization
├─ Reference reporting relationships
└─ Establish interview purpose

Phase 2: Core Responsibilities Discovery (40%)
├─ Open-ended exploration
├─ Task frequency identification
├─ Priority ranking
└─ Time allocation mapping

Phase 3: Interaction Mapping (25%)
├─ Internal stakeholder identification
├─ External touchpoints
├─ Communication patterns
└─ Approval workflows

Phase 4: Edge Cases & Variations (15%)
├─ Seasonal variations
├─ Exception handling
├─ Crisis responsibilities
└─ Growth/scaling tasks

Phase 5: Validation & Refinement (10%)
├─ Summary confirmation
├─ Gap identification
└─ Cross-reference with hierarchy
```

**Sample Opening Pattern:**
```
"I understand you serve as [Position] reporting to [Manager Position] 
and collaborating closely with [Related Positions]. I'd like to learn 
about your day-to-day responsibilities and how your work contributes 
to [Department/Company Goal]. Could we start with what a typical week 
looks like for you?"
```

---

## Problem 2: Optimal Worklist Extraction Method

### Solution: Multi-Layer Extraction Framework

#### **Method: Temporal-Categorical Hybrid Approach**

### Layer 1: Temporal Decomposition

**Daily Tasks**
- Opening routines
- Continuous monitoring activities
- End-of-day closeouts
- Time-sensitive responsibilities

**Weekly Tasks**
- Recurring meetings and reporting
- Review cycles
- Team synchronization activities
- Planning sessions

**Monthly Tasks**
- Performance reviews
- Budget activities
- Strategic planning
- Compliance and audit items

**Quarterly/Annual Tasks**
- Goal setting and reviews
- Major planning initiatives
- Seasonal variations
- Annual compliance

### Layer 2: Categorical Extraction

```
1. OPERATIONAL TASKS
   ├─ Routine operations
   ├─ Process execution
   └─ Quality control

2. MANAGEMENT TASKS
   ├─ Team supervision
   ├─ Performance management
   └─ Resource allocation

3. COMMUNICATION TASKS
   ├─ Stakeholder updates
   ├─ Cross-functional coordination
   └─ Reporting obligations

4. STRATEGIC TASKS
   ├─ Planning and forecasting
   ├─ Initiative development
   └─ Improvement projects

5. ADMINISTRATIVE TASKS
   ├─ Documentation
   ├─ System updates
   └─ Compliance activities
```

### Extraction Question Framework

**Discovery Questions:**
```
Scope Questions:
- "What are your primary responsibilities?"
- "What deliverables are you accountable for?"

Frequency Questions:
- "Which tasks require daily attention?"
- "What do you handle on a weekly/monthly basis?"

Dependency Questions:
- "Whose input do you need to complete this?"
- "Who depends on this output from you?"

Priority Questions:
- "What must be done versus what's nice to have?"
- "What happens if this task is delayed?"

Context Questions:
- "Are there busy seasons or slower periods?"
- "What changes during quarter-end?"
```

### Extraction Best Practices

1. **Use Specific Probes**: Replace "What do you do?" with "Walk me through your Monday morning routine"

2. **Trigger Examples**: Leverage LLM knowledge to prompt memory
   - "Store managers typically handle inventory counts—how do you approach this?"

3. **Cross-Reference Validation**: Compare against:
   - Upstream position outputs
   - Downstream position needs
   - Similar positions in other departments

4. **Capture Task Attributes**:
   ```
   Task: [Name]
   ├─ Frequency: [Daily/Weekly/Monthly/Quarterly/Annual/Ad-hoc]
   ├─ Duration: [Time required]
   ├─ Priority: [Critical/High/Medium/Low]
   ├─ Dependencies: [Prerequisites/Inputs needed]
   ├─ Outputs: [Deliverables/Artifacts]
   ├─ Stakeholders: [Who's involved/informed]
   └─ Tools: [Systems/Resources used]
   ```

---

## Problem 3: Conflict-Free Conversational Design

### Solution: Structured Conflict Prevention Framework

#### **Strategy: Hierarchical Context-Aware Interviewing**

### Conflict Prevention Mechanisms

#### 1. **Interview Sequencing Strategy**

```
Recommended Order:
1. Executive/Leadership layer
   └─ Establishes strategic context and priorities

2. Department heads
   └─ Defines functional boundaries and objectives

3. Mid-level managers
   └─ Captures coordination and tactical execution

4. Individual contributors
   └─ Details operational reality and ground truth
```

**Benefit**: Upper-level context prevents misalignment in lower-level interviews

#### 2. **Conflict Detection Patterns**

**Monitor for these red flags:**

```yaml
Task Ownership Conflicts:
  Pattern: "Multiple positions claiming primary ownership"
  Resolution: "Clarify decision rights vs. execution rights"

Reporting Discrepancies:
  Pattern: "Position claims reporting to X, but structure shows Y"
  Resolution: "Validate with organizational chart, identify matrix reporting"

Dependency Mismatches:
  Pattern: "Position A says they provide X to Position B, but B doesn't mention it"
  Resolution: "Explicit validation: 'Position A mentioned they provide X—do you use this?'"

Timeline Conflicts:
  Pattern: "Incompatible task frequencies (daily report vs. weekly input)"
  Resolution: "Clarify actual cadence and buffer mechanisms"
```

#### 3. **Conflict Resolution Protocol**

```
When conflict detected:

Step 1: Document both perspectives
  └─ "You mentioned X, but [Position] indicated Y"

Step 2: Identify root cause
  ├─ Terminology difference?
  ├─ Process evolution (outdated knowledge)?
  ├─ Actual gap/inefficiency?
  └─ Shadow/informal processes?

Step 3: Validate with hierarchy
  └─ "According to [Manager], this responsibility sits with..."

Step 4: Update both records
  └─ Ensure consistency across related position interviews
```

#### 4. **Consistency Validation Checkpoints**

```
After every interview:

□ Cross-check mentioned upstream dependencies
□ Verify downstream consumers of outputs
□ Validate meeting/communication touchpoints
□ Confirm approval workflows
□ Check task frequencies against calendar realities
```

#### 5. **Diplomatic Phrasing Guide**

**Instead of challenging directly, use:**

| Confrontational | Diplomatic Alternative |
|----------------|----------------------|
| "That contradicts what I heard" | "Help me understand how this aligns with..." |
| "You're wrong about that" | "I want to make sure I captured this correctly..." |
| "That's not your responsibility" | "Where does your role end and [Position] begin?" |
| "You didn't mention X" | "Does X fall within your scope?" |

#### 6. **Ambiguity Resolution Techniques**

**When boundaries are unclear:**

```
"Let's map out a specific scenario:
 
When [Event X] happens:
1. Who makes the initial decision?
2. Who needs to be consulted?
3. Who implements it?
4. Who verifies completion?
5. Who reports the outcome?

This helps us clarify where your responsibility starts and ends."
```

---

## Implementation Workflow

### Step-by-Step Process

```
1. PRE-INTERVIEW PREPARATION
   ├─ Load organizational structure
   ├─ Review position in hierarchy
   ├─ Load LLM general knowledge for position type
   ├─ Review previous related position interviews
   └─ Prepare conflict checkpoints

2. INTERVIEW EXECUTION
   ├─ Context Setting (introduce purpose, establish rapport)
   ├─ Temporal Discovery (daily → weekly → monthly → periodic)
   ├─ Categorical Deep Dive (operational → management → strategic)
   ├─ Relationship Mapping (upstream → downstream → lateral)
   └─ Edge Case Exploration (exceptions, variations, growth)

3. REAL-TIME VALIDATION
   ├─ Cross-reference against org structure
   ├─ Flag potential conflicts
   ├─ Verify dependencies with previous interviews
   └─ Identify gaps requiring follow-up

4. POST-INTERVIEW PROCESSING
   ├─ Compile comprehensive worklist
   ├─ Categorize and prioritize tasks
   ├─ Resolve flagged conflicts
   ├─ Update dependency map
   └─ Store as context for future interviews

5. QUALITY ASSURANCE
   ├─ Manager review of subordinate worklists
   ├─ Cross-functional validation
   ├─ Identify missing handoffs
   └─ Finalize position documentation
```

---

## Sample Interview Transcript Pattern

```
CLAUDE: I understand you're the Store Manager reporting to the Regional 
Director and working closely with Assistant Managers and Department Leads. 
I'd like to understand your complete worklist to document how your role 
contributes to store operations. Shall we start with your daily routines?

POSITION: Sure, I start each day with...

CLAUDE: That's helpful. You mentioned opening procedures—how long does 
that typically take, and what must be completed before the store opens?

POSITION: Usually 30-45 minutes. I need to...

CLAUDE: I see you work with inventory data. The Inventory Lead mentioned 
they provide you with daily stock reports—is that something you review 
during opening procedures?

[Validation checkpoint: Cross-referencing with Inventory Lead interview]

POSITION: Yes, that's one of my key morning tasks...

CLAUDE: Perfect. Now thinking about your weekly cycle, what recurring 
responsibilities do you have?

[Temporal progression: Daily → Weekly]
```

---

## Output Quality Metrics

### Comprehensive Worklist Should Include:

- [ ] **Completeness**: All task categories covered
- [ ] **Specificity**: Concrete tasks, not vague descriptions
- [ ] **Temporality**: Clear frequency for each task
- [ ] **Dependencies**: Inputs and outputs mapped
- [ ] **Stakeholders**: All touchpoints identified
- [ ] **Validation**: Cross-referenced with related positions
- [ ] **Consistency**: No conflicts with organizational structure
- [ ] **Measurability**: Deliverables and metrics defined

---

## Advanced Considerations

### Handling Complex Scenarios

**Matrix Organizations**
- Multiple reporting lines require explicit clarification
- Map decision rights vs. execution rights separately
- Document percentage allocation to different functions

**Rapidly Growing Companies**
- Flag tasks that will shift as company scales
- Identify tasks ripe for delegation
- Note transitional responsibilities

**Seasonal Businesses**
- Create separate worklists for peak vs. off-peak
- Document ramp-up and wind-down tasks
- Identify hiring/training seasonality

**Remote/Hybrid Teams**
- Capture communication frequency and modalities
- Identify asynchronous vs. synchronous requirements
- Document coordination mechanisms

---

## Conclusion

This framework ensures:
✓ Systematic extraction of comprehensive worklists  
✓ Conflict-free documentation through validation  
✓ Consistent organizational understanding  
✓ Scalable process for any company size  
✓ Reusable context for future analysis

The conversational approach balances thoroughness with natural dialogue, making the interview collaborative rather than interrogative while maintaining the structure needed for complete worklist extraction.