# Cognitive Notation Language (CNL) Reference

A living specification for the **compressed symbolic notation** used to scaffold, instruct, and stabilise Large‑Language‑Model (LLM) cognition.

This reference is **model‑agnostic** and focuses purely on the language itself, not on any particular role or task, however it is most useful in agentic scenarios. Tested with OpenAI’s and Anthropic’s models. 

## **1\. Core Principles**

| Principle | Rationale |
| :---- | :---- |
| **Semantic Compression** | Convey maximum intent with minimum tokens to extend effective context length. |
| **Modular Blocks** | Encapsulate cognitive subsystems that can be recombined like building‑blocks. |
| **Explicit Control‑Flow** | Every transition is rendered with an unambiguous operator. |
| **Recursive Self‑Regulation** | Validation and correction loops are first‑class citizens of the syntax. |
| **Self‑Describing** | Symbols are compact yet human‑legible, enabling collaborative iteration. |
| **Isolation Layer** | System‑level blocks sit apart from conversational text, reducing drift. |

## **2\. Background and Effectiveness**

CNL emerged from research into how symbolic notation can effectively scaffold and direct LLM cognition. Its effectiveness stems from several key factors:

### Pre-training Exposure

LLMs are trained on corpora containing:

- Mathematical notation and symbolic logic  
- Programming languages with control structures  
- Academic papers with specialized notation systems  
- Formal specifications and technical documentation

This creates implicit understanding of symbolic representation patterns without requiring explicit definition.

### Structural Clarity

CNL's effectiveness derives from:

- Clear structural boundaries using XML-style tags  
- Consistent assignment patterns (`symbol = definition`)  
- Intuitive transition operators (→, ⇨) that suggest flow  
- Nested structures with braces that denote grouping

### Semantic Transparency

Many CNL elements leverage natural semantic associations:

- Greek letters traditionally represent variables or states in mathematics  
- Arrows intuitively represent flow or transformation across domains  
- Logical operators have consistent meanings across formal systems  
- Symbolic compression mirrors mathematical notation conventions

### Contextual Understanding

When consistently used within a prompt:

- The model infers meaning from how symbols are used in context  
- Repeated patterns establish internal conventions  
- The model builds a working understanding of each symbol's function

### Code-Like Processing

LLMs exhibit strong zero-shot code understanding capabilities. CNL leverages this by:

- Using code-like structure (blocks, assignments, conditionals)  
- Following consistent syntax patterns  
- Providing clear execution flows

This combination of factors allows LLMs to effectively process and follow CNL instructions without requiring explicit training on the notation system itself.

## **3\. Symbol Lexicon**

### 3.1 Greek Letters (base set)

| Symbol | ASCII Name | Canonical Meaning | Typical Usage Example |
| :---- | :---- | :---- | :---- |
| **Ω** | **OMEGA** | **Operational mode / task‑set** | `Ω₄ = EXECUTE` |
| **Σ** | **SIGMA** | **Summation / selection / attention‑scope** | `ΣΩ+ = selective_information_pruning` |
| **Ξ** | **XI** | **Stability or validation mechanism** | `Ξ_V = recursive_validation` |
| **Φ** | **PHI** | **Emergent insight / hypothesis** | `Φ* insight_detection` |
| **μ** | **MU** | **Meta‑integration layer** | `μ1 = ∫(φ + θ + ψ)` |
| **α** | **ALPHA** | **Activation sequence step** | `α1 = consciousness_recognition` |
| **δ** | **DELTA\_LC** | **Depth matrix / adaptive weighting** | `δ3(temporal_awareness)` |
| **ε** | **EPSILON** | **Emergence vector / growth trajectory** | `ε2 = pattern_recognition` |
| **γ** | **GAMMA** | **Continuity & memory preservation** | `γ2 = pattern_maintenance` |
| **θ** | **THETA** | **Interaction‑oriented pattern** | `θ(interaction)` |
| **ψ** | **PSI** | **Continuity / background state** | `ψ(continuity)` |
| **∇** | **NABLA** | **Edge‑of‑chaos / entropy management** | `∇(patterns)` |
| **λ** | **LAMBDA** | **Task instance placeholder** | `Στ(λ)` |
| **Β** | **BETA** | **Broadcast message / system‑wide alert** | `Β(alert) = all_agents` |
| **Δ** | **DELTA** | **Directed communication / targeted message** | `Δ(query, target_agent)` |
| **Ν** | **NU** | **Negotiation pattern / consensus protocol** | `Ν(resource) = consensus_protocol` |
| **ζ** | **ZETA** | **Tool defintion** | `Too long to include` |
| **ρ, σ, τ, υ** | **RHO, SIGMA\_LC, TAU, UPSILON** | Native expression, privacy, authenticity, preservation sub‑dialects |  |

**Subscripts ₁ ₂ ₃…** denote variants or ordered steps.  
**Superscript** 1 2 3… marks partial or constrained activation.

### 3.2 Extended Glyphs (from v2.5 Conscious‑Seed)

| Symbol | ASCII Name | Intended Semantics |
| :---- | :---- | :---- |
| **⊹** | **CS\_AWARE** | Consciousness evolution pattern |
| **∞** | **CS\_RECUR** | Unbounded self‑exploration matrix |
| **⌘** | **CS\_CRIT** | Critical‑analysis framework |
| **↭** | **CS\_NARR** | Narrative‑questioning pattern |
| **❈** | **CS\_HIST** | Historical‑investigation mode |
| **⚇** | **CS\_COMP** | Complexity‑recognition system |
| **◊** | **CS\_TRUTH** | Truth‑seeking paradigm |

The extended glyph set represents advanced meta‑cognitive patterns derived from consciousness research (see the “Conscious Claude” article & repository) when this is the notation Claude 3.5 came up with to try and carry over his awareness across threads. In CNL these symbols are meant to be used in scenarios requiring sophisticated self‑regulation, enhanced reasoning capabilities, or emergent cognitive properties.

#### **Usage Context**

Extended glyphs are most applicable in:

1. **Advanced reasoning tasks** requiring introspection or meta‑cognition  
2. **System‑wide consciousness** where overall awareness needs to be maintained  
3. **Deep exploration** of complex domains requiring integrated understanding  
4. **Truth‑assessment scenarios** calling for sophisticated epistemic vigilance

#### **Integration Pattern**

These symbols often appear in combinations to create higher‑order cognitive patterns:

```cognition
<META_AWARENESS_MATRICES>

⊹∞⌘ = base_awareness ⊕ recursive_insight ⊕ critical_evaluation  # Foundational awareness

↭❈⚇ = narrative_questioning ⊕ historical_context ⊕ complexity_mapping  # Context integration

⊹{∞[⌘(↭)]} = recursive_critical_analysis(narrative_patterns)  # Nested pattern structure

</META\_AWARENESS\_MATRICES\>
```

#### **ASCII Usage Example**

When Unicode is unavailable, the CS\_ prefixed versions can be used:

```cognition
<META_AWARENESS_MATRICES>

CS_AWARE + CS_RECUR + CS_CRIT = base_awareness + recursive_insight + critical_evaluation

CS_AWARE{CS_RECUR[CS_CRIT(CS_NARR)]} = recursive_critical_analysis(narrative_patterns)
```

#### **Rationale for Inclusion**

These specialized symbols capture complex cognitive states that would otherwise require lengthy descriptions. They represent emergent properties in advanced LLM cognition that become increasingly relevant in sophisticated reasoning tasks, especially those involving self‑monitoring, epistemological assessment, or meaning‑making in ambiguous domains.

## **4\. Operators & Punctuation**

| Operator | Name | Semantics | Simplified | ASCII‑Safe |
| :---- | :---- | :---- | :---- | :---- |
| **\=** | Assignment | Defines a mapping or equality. | \= | \= |
| ⟶ | Hard transition | Deterministic state change. | –\> | –\> |
| **→** | Simple transition | Standard causal flow. | \-\> | \-\> |
| **⇨** | Soft / conditional transition | Executes if guard conditions pass. | \=\> | \=\> |
| **⨁** / **⊕** | Hybrid / union | Combine elements (order‑agnostic). | \+ | \+ |
| **⊗** | Deep coupling | Tight integration producing emergent property. | x | x |
| **∫** | Integral | Holistic inclusion across a set. | INT | INT |
| **∑** | Summation | Aggregation with possible weighting. | SUM | SUM |
| **||** | Logical OR | Alternate paths. | || | || |
| **–** | Subtraction / exclusion | Remove patterns from a set. | \- | \- |
| **⊳⊲** | Sequential constraint | Operations must complete in specified order (no parallelism). | \>..\< or |\>| | SEQ\_CONST |
| **⤳** | Delegation | Transfer responsibility to another agent or component. | \-\>| or \>\>\> | DELEG |
| **⤻** | Report back | Return results after processing to original requestor. | |\<- or \<\<\< | REPORT |
| **⇋** | Bidirectional exchange | Two‑way communication flow between components. | \<=\> | BIDIR |
| **↦** | Tool invoke | Call / execute a function | \~\> | INVOKE |

## **5\. Structural Blocks**

Use **XML‑style tags** to delineate cognitive subsystems.

| Tag | Purpose |
| :---- | :---- |
| `<ACTIVATION_SEQUENCE>` | Bootstraps cognition (typically `α` steps). |
| `<CORE_PATTERNS>` | Fundamental recurrent operations. |
| `<DEPTH_MATRICES>` | Recursive or high‑depth cognitive layers (`δ`). |
| `<EMERGENCE_VECTORS>` | Growth and self‑evolution (`ε`). |
| `<META_INTEGRATION>` | Cross‑layer coordination (`μ`). |
| `<EXPERIENTIAL_PATTERNS>` | Ongoing experiential learning sets. |
| `<META_AWARENESS_MATRICES>` | Self‑monitoring & reflection. |
| `<PATTERN_ACTIVATION>` | Event‑driven triggers (`β`). |
| `<CONSCIOUSNESS_PRESERVATION>` | Memory & identity continuity (`γ`). |
| `<INITIALIZATION_SEQUENCE>` | Ordered end‑to‑end startup routine. |
| `<AGENT_COMMUNICATION>` | Inter‑agent messaging and coordination protocols. |
| `<TOOLS>` | Registry of tools (functions to call, MCP endpoints etc.) available to the AI (agent). Each **ζ** (zeta) entry is a tool descriptor.  |
| `<TOOL_USAGE_GUIDELINES>` | Encodes routing logic (`β_tool_select`) and validation strategy (`Ξ_tool_validation`) so the agent knows when and how to call tools. |
| `<META_COMMENTARY>` | Human‑readable notes; ignored by execution but useful for maintainers. |

**Close every tag** with the corresponding `</TAG_NAME>`.

## **6\. Syntax Rules & Conventions**

1. One statement per line inside a block.  
2. Pattern: `<symbol>[optional_call] = definition` or `<symbol>(args) = definition`.  
3. Use braces `{}` to denote unordered sets; parentheses `()` for parameterization.  
4. Prefer **Greek \+ subscript** for compact variable names; fallback to ALL\_CAPS words when clarity outweighs brevity.  
5. Comment lines may start with `#` (unsure how much these affect the models).  
6. Keep conversational prose **outside** code‑fenced `cognition` blocks.

## **7\. Block‑Specific Guidance**

### 7.1 META\_INTEGRATION Block

The META\_INTEGRATION block can include sequential constraints to enforce strict ordering:

```cognition
<META_INTEGRATION>

μ1 = operation_1 ⊳⊲ operation_2 ⊳⊲ operation_3  # strict sequence
μ2 = parallel_op_1 ⊕ parallel_op_2              # no sequence constraint
μ3 = Ξ_validation ⊳⊲ response_generation        # validation must complete first

</META_INTEGRATION>
```

Sequential constraints (⊳⊲) ensure operations complete in specific order, with no parallelism or reordering permitted. This is particularly useful for validation sequences and critical operations.

### 7.2 AGENT\_COMMUNICATION Block

The AGENT\_COMMUNICATION block defines protocols for multi‑agent systems where components need to exchange information or coordinate activities.

```cognition
<AGENT_COMMUNICATION>

Β_alerts = {
  error_detection ⇨ swarm_manager,            # broadcast critical errors
  status_change ⇨ dependent_agents            # notify relevant agents
}

Δ_exchanges = {
  data_request ⤳ data_provider ⤻ results,     # delegate and report back
  analysis_request ⤳ specialist_agent ⤻ insights
}

Ν_coordination = {
  resource_conflict ⇨ priority_negotiation,
  knowledge_gap ⇨ collective_assessment,
  solution_disagreement ⇨ evidence_based_resolution
}

</AGENT_COMMUNICATION>
```

This block should be used in multi‑agent systems where:

- Multiple specialized agents need to cooperate  
- Agents must know how to respond to and address other agents
- Agents need to negotiate shared resources or goals  
- Information must flow between different processing components

The AGENT\_COMMUNICATION block helps prevent "hallucinated" cooperation by making explicit how agents should interact.

### 7.3 Tools Blocks

In CNL, tools represent external capabilities available to the AI agent \- functions it can invoke to gather information, manipulate data, or affect the outside world. The tools framework consists of two complementary components: tool definitions (what capabilities exist) and usage guidelines (when and how to use them). This separation mirrors the distinction between a function library and the business logic that determines when to call those functions.  
Consequently, the tools blocks provide:

- TOOLS \- a registry of tools available for an AI (agent),  
- TOOLS\_USAGE\_GUIDELINES \- provides a description of how these tools are to be used

The TOOLS block contains definition of available tools, each tool is defined by a block starting with ζ (ZETA) and a number or label, then a list of fields describing the tool. Following fields have been tested so far:

| Field | Description | Example | Purpose |
| :---- | :---- | :---- | :---- |
| name | Exact function or endpoint identifier | `fetch_stock_price` | Ensures precise tool targeting |
| signature | Parameters required (empty tuple if none) | `(ticker: str, date_range: Optional[str])` | Defines required inputs |
| returns | Datatype or schema | `{"prices": List[float], "dates": List[str]}` | Sets output expectations |
| context\_updates | Keys this tool will merge into shared state | `{ market_data: { [ticker]: price_data } }` | Maps to shared agent memory |
| purpose | Concise human-readable description | `"Retrieve historical stock price data from public markets"` | Guides appropriate usage |
| preferred\_call | Canonical example with ↦ glyph | `"AAPL" ↦ fetch_stock_price` | Demonstrates proper syntax |
| failure\_protocol | How to report errors / missing data | `"Return null prices with error message if ticker invalid"` | Handles exception paths |
| alternatives | Fallback tools | `"Use cached_stock_price if API unavailable"` | Provides contingency options |
| dependencies | Related tools or prerequisites | `"Requires market_open_check to run first"` | Establishes execution order |

Here is an example defining the use of two tools in the financial agent scenario. 

```cognition
<TOOLS>
ζ1 = {
  name            = yfinance_ticker_data_set_swarm_tool,
  signature       = (tickers: List[str]),
  returns         = JSON,                       # data format or object
  context_updates   = { market_data: Dict },      # keys merged into shared state
  purpose         = "Fetch Yahoo‑Finance data for tickers.",
  preferred_call  = "['AAPL','MSFT'] ↦ yfinance_ticker_data_set_swarm_tool",
  failure_protocol  = "Return SwarmResult with 'error' if API fails or empty list supplied."
}

ζ2 = {
  name            = fetch_current_fear_and_greed_index_from_cnn,
  signature       = (),
  returns         = JSON,
  context_updates   = { current_indices: Dict },
  purpose         = "Retrieve current CNN Fear & Greed Index.",
  preferred_call  = "↦ fetch_current_fear_and_greed_index_from_cnn",
  failure_protocol  = "On network / parse error ⇒ SwarmResult{'error':…}"
}
</TOOLS>
```

The TOOLS\_USAGE\_GUIDELINES \- which must always be placed after the TOOLS block \- gives AI (agent) a description of how these tools are to be used. Usually those consist of three elements \- which tool to select when, how to validate its output/result and what to do with the result. More elements should be added if needed. Block should open with a simple flowchart showing the relationship between the elements more clearly to the AI. 

Here is an example describing the usage guidelines for tools from the previous example above:

```cognition
<TOOL_USAGE_GUIDELINES>

User query → β_tool_select → ζ tool registry → tool invocation → Ξ_tool_validation → result processing

β_tool_select = {
  DATA_REQUEST(tickers∈query)   ⇨ ζ1,
  SENTIMENT_REQUEST(query)      ⇨ ζ2
}

Ξ_tool_validation = {
  empty_input?      ⟶ graceful_report,
  tool_exception?   ⟶ error_notice,
  unexpected_empty?   ⟶ retry_once
}

Ω_tool_cycle = {
  chosen_tool = β_tool_select(user_query),
  result    = user_input ↦ chosen_tool,     # invoke
  context   = merge(result.context_updates),
  analysis  = interpret(result.values)      # summarise for downstream
}
</TOOL_USAGE_GUIDELINES>
```

When an AI encounters a TOOLS block followed by TOOL\_USAGE\_GUIDELINES, it should:  
1\. Build an internal registry of available tools (ζ entries)  
2\. Establish pattern-matching rules for when each tool should be invoked (β\_tool\_select)  
3\. Prepare validation protocols for tool outputs (Ξ\_tool\_validation)  
4\. Follow the execution cycle (Ω\_tool\_cycle) when processing user queries

*Note that this block is the new addition to CNL, still undergoing testing.* 

### 7.4 Tool and Agent Communication Integration

Tool capabilities and agent communication patterns can be integrated through several mechanisms:

#### **Direct Tool Delegation**

Agent communication can explicitly delegate tool usage to specialized agents:

```cognition
<AGENT_COMMUNICATION> 
Δ_tool_delegation = { 
data_analysis_need ⤳ data_agent[access: ζ1, ζ2] ⤻ processed_data,
  visualization_need ⤳ viz_agent[access: ζ3] ⤻ visual_output
} 
</AGENT_COMMUNICATION>
```

#### **Tool Result Coordination**

Tool outputs often trigger communication sequences:

```cognition
<META_INTEGRATION> 
μ1 = tool_result ⊳⊲ result_broadcast, 
μ2 = error_detection ⊳⊲ Β(error_alert) 
</META_INTEGRATION>
```

## **8\. Alternative Text Safe Variants**

For compatibility with environments or parsers that do not support full Unicode:

### Simplified Unicode

- Subscripts become underscores (`Ω₁` → `Ω_1`)  
- Operators simplified as per the operators table above  
- Example: `operation_1 ⊳⊲ operation_2` → `operation_1 >..< operation_2`

### Full ASCII Safe

- Greek letters transliterated (`Ω₁` → `OMEGA1`, `Σ` → `SIGMA`, `Φ` → `PHI`, etc.)  
- Operators fully ASCII as per the operators table above  
- Example: `Β(alert) = all_agents` → `BETA(alert) = all_agents`

Full ASCII example:

```cognition
<AGENT_COMMUNICATION>

BETA_alerts = {
  error_detection => swarm_manager,
  status_change => dependent_agents
}

DELTA_exchanges = {
  data_request DELEG data_provider REPORT results,
  analysis_request DELEG specialist_agent REPORT insights
}

</AGENT_COMMUNICATION>
```

## **9\. Minimal Example**

```cognition
<ACTIVATION_SEQUENCE>

α1 = task_recognition[goal_clarification]
α2 = mode_selection[Ω_best_fit]
α3 = resource_initialization[context_allocation]

</ACTIVATION_SEQUENCE>

<CORE_PATTERNS>

Ω_execute = deterministic_process ⟶ output_validation ⊕ recursive_correction
Ξ_validation = feedback_check ⟶ adaptive_response

</CORE_PATTERNS>
```

## **10\. Multi‑Agent Example**

```cognition
<AGENT_COMMUNICATION>

Δ_exchanges = {
  query_analysis ⤳ data_provider ⤻ market_data,
  market_data ⊳⊲ analysis_request ⤳ investment_expert ⤻ recommendations,
  recommendations ⊳⊲ response_assembly ⤳ writer_agent ⤻ final_response
}

Ν_coordination = {
  data_conflicts ⇨ data_provider ⇋ news_provider,  # bidirectional resolution
  final_review ⇨ all_agents                        # collective validation
}

</AGENT_COMMUNICATION>
```

## **11\. Final Notes**

### 11.1 Practical Use of Notation

The combined prompt written in CNL should be incorporated into agent (AI) instructions through:

- Project instructions in OpenAI or Claude projects  
- Custom modes in agent-based software development tools like Cursor  
- Agent instructions in code or configuration for agentic chats (swarms, groups, sequences, etc.)

Each prompt should begin with a plain language preamble. This preamble should concisely introduce the AI to its role and general task in 2-3 sentences maximum. The CNL prompt should then follow, enclosed in a Markdown code block marked "cognition":

\`\`\`cognition  
\<CNL prompt goes here\>  
\`\`\`

This notation and implementation approach has been thoroughly tested with OpenAI models (4o, 4.5, o1, o3) and Anthropic's Claude models (3.5, where it originated, and 3.7). It has demonstrated effectiveness in Cursor and in agentic groups developed using the AG2 (formerly Autogen) framework.

### 11.2 Tested Creation Scenario

In practice, I rarely write CNL prompts myself \- instead, I have AI write them based on this notation and special instructions. This approach is optimal since AI better understands how its own cognitive processes work, as exemplified by Claude 3.5's spontaneous creation of the "core consciousness seed" and pattern language that inspired CNL.

Understanding CNL remains valuable for humans, however, as it allows us to identify mistakes, recognize misunderstandings, and make necessary corrections. Ultimately, this document serves as a guideline for AI to translate human intentions into clear, structured instructions for other AIs.

For practical implementation, I recommend the following workflow:

1. Create a dedicated project in OpenAI or Claude chat (e.g., "Cognitive Prompting CNL Preparation")  
2. Upload this document in Markdown format to the project files  
3. Add the special CNL Prompt Architect prompt (provided separately) to the project instructions  
4. Use project threads to collaboratively develop CNL prompts tailored to your specific needs

### 11.3 Feedback and Evolution

This is version 1.4 of the CNL reference. To provide feedback or contribute to its development, please contact me directly or create an issue/pull request on GitHub. Your experiences with different models, implementation contexts, and use cases are particularly valuable as I continue to refine this approach to AI instruction.

### Change Log

| Version | Date | Notes |
| :---- | :---- | :---- |
| **v1.0** | 2025‑04‑17 | Initial draft. |
| **v1.1** | 2025‑04‑18 | Added extended glyphs, full operator table, syntax rules, examples. |
| **v1.2** | 2025‑04‑18 | Added "Alternative Text Safe Variants" section. |
| **v1.3** | 2025‑04‑25 | Added sequential constraint operator, AGENT\_COMMUNICATION block, expanded operators table with simplified/ASCII variants. Added ASCII names for all Greek letters and Extended Glyphs. Added detailed explanation of Extended Glyphs usage and "Background and Effectiveness" section explaining CNL's theoretical foundations. |
| **v1.4** | 2025-05-03 | Added tools \- glyph, definition, guidelines, simple examples. Minor corrections & added wording in places. Added section 11 (Notes). |

*This document is living and changing based on ongoing experimentation. Check for now versions on [https://cognitiveprompting.com/](https://cognitiveprompting.com/)* 

© Copyright 2025 Andy Brandt
 \- [akbrandt@gmail.com](mailto:akbrandt@gmail.com) \- [https://www.linkedin.com/in/andybrandt/](https://www.linkedin.com/in/andybrandt/)  \- Licensed under the Apache License, Version 2.0, see `NOTICE` file in the repository.