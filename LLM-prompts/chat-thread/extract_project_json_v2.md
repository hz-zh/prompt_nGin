# Project Documentation Extraction Prompt

## Objective
Generate a comprehensive, technically-oriented JSON summary of this project session that captures all development details, methodological approaches, and chronological progression for LLM-assisted documentation generation.

## Output Requirements

### JSON Structure Requirements
- **Hierarchical Organization**: Structure data chronologically with nested technical details
- **Technical Density**: Prioritize technical descriptions over general summaries  
- **Granular Detail**: Create subfields rather than combining information
- **Complete Coverage**: Include all discussed points, implementations, and iterations

### Required Top-Level Sections

#### 1. Project Metadata
```json
{
  "project_identification": {
    "name": "string",
    "repository_path": "string",
    "session_timestamp": "ISO8601",
    "primary_domain": "string",
    "development_stage": "string"
  }
}
```

#### 2. Technical Implementation Sequence
```json
{
  "implementation_chronology": [
    {
      "iteration_number": "integer",
      "timestamp_relative": "string",
      "technical_approach": {
        "method_description": "detailed technical process",
        "algorithm_specifics": "step-by-step technical details",
        "data_structures": ["list of structures used"],
        "key_functions": ["function names and purposes"]
      },
      "code_artifacts": {
        "files_modified": ["filepath list"],
        "new_capabilities": ["capability descriptions"],
        "performance_characteristics": "string"
      }
    }
  ]
}
```

#### 3. Current Technical State
```json
{
  "final_implementation": {
    "core_methodology": "detailed technical description",
    "system_architecture": "architectural overview",
    "data_flow": "step-by-step data processing",
    "key_algorithms": {
      "algorithm_name": "technical description without code"
    },
    "performance_metrics": "quantitative measures if available"
  }
}
```

#### 4. Development Evolution
```json
{
  "method_iteration_sequence": [
    {
      "version": "string",
      "changes_made": "specific technical changes",
      "rationale": "reasoning for changes",
      "improvements_achieved": "measurable improvements",
      "challenges_addressed": "technical problems solved"
    }
  ]
}
```

## Formatting Standards

### Detail Preservation
- **NO INFORMATION LOSS**: Every technical detail mentioned must be captured
- **SEPARATE SUBFIELDS**: Create distinct fields for each concept rather than combining
- **MAINTAIN SPECIFICITY**: Preserve exact technical terminology and specifications
- **CHRONOLOGICAL INTEGRITY**: Maintain temporal sequence of all developments

### Technical Description Standards
- Focus on **HOW** the system works, not **WHAT** the code looks like
- Include algorithmic approaches, data transformations, and system behaviors
- Specify input/output relationships and processing steps
- Document decision points and optimization strategies

## Validation Criteria
Before submission, ensure:
- [ ] All chat session content is represented
- [ ] Technical processes are described in implementation detail
- [ ] Chronological sequence is maintained throughout
- [ ] No combining of distinct concepts or approaches
- [ ] JSON structure is valid and complete
- [ ] Each iteration/change is individually documented

## Output Format
Provide a single, valid JSON object containing all required sections with maximum technical detail and chronological accuracy.