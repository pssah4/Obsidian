---

database-plugin: basic

---

```yaml:dbfolder
name: Data Base
description: Filterbare Vault Datenbank
columns:
  __file__:
    key: __file__
    id: __file__
    input: markdown
    label: File
    accessorKey: __file__
    isMetadata: true
    skipPersist: false
    isDragDisabled: false
    csvCandidate: true
    position: 1
    isHidden: false
    sortIndex: -1
    width: 309
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: true
      task_hide_completed: true
      footer_type: none
      persist_changes: false
      content_alignment: text-align-left
  Summary:
    input: text
    accessorKey: Summary
    key: Summary
    id: Summary
    label: Summary
    position: 2
    skipPersist: false
    isHidden: false
    sortIndex: -1
    width: 469
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
      content_alignment: text-align-left
  tags:
    input: tags
    accessorKey: tags
    key: tags
    id: tags
    label: tags
    position: 4
    skipPersist: false
    isHidden: true
    sortIndex: -1
    options:
      - { label: "AI,Klimawandel,draft", value: "AI,Klimawandel,draft", color: "hsl(216, 95%, 90%)"}
      - { label: "ChatGPT,Perplexity,GPT,Reasoning,draft", value: "ChatGPT,Perplexity,GPT,Reasoning,draft", color: "hsl(240, 95%, 90%)"}
      - { label: "draft,GPT,OpenAI,Prompting,AI,Technologie", value: "draft,GPT,OpenAI,Prompting,AI,Technologie", color: "hsl(226, 95%, 90%)"}
      - { label: "AI,Agents,Technologie,draft", value: "AI,Agents,Technologie,draft", color: "hsl(115, 95%, 90%)"}
      - { label: "Digitalisierung,Energiewirtschaft,Datenökosysteme,Energiedatenräume,Gaia-X,IT-Architektur,energydata-X,EnBW,Initiative,These,Blockchain", value: "Digitalisierung,Energiewirtschaft,Datenökosysteme,Energiedatenräume,Gaia-X,IT-Architektur,energydata-X,EnBW,Initiative,These,Blockchain", color: "hsl(231, 95%, 90%)"}
      - { label: "Prompting,OpenAI,Anthropic,draft,Technologie", value: "Prompting,OpenAI,Anthropic,draft,Technologie", color: "hsl(76, 95%, 90%)"}
      - { label: "AI,Softwareentwicklung,Automatisierung,Agenten,Entwicklerproduktivität,Infrastruktur,Cloud,GitHub,Copilot,Microsoft,Arbeitswelt,Produktivität,OpenSource,Coding,Content", value: "AI,Softwareentwicklung,Automatisierung,Agenten,Entwicklerproduktivität,Infrastruktur,Cloud,GitHub,Copilot,Microsoft,Arbeitswelt,Produktivität,OpenSource,Coding,Content", color: "hsl(37, 95%, 90%)"}
      - { label: "AI,Wirtschaft,Gesellschaft,Technologiewandel,Arbeitsmarkt,Produktivität,Innovation,Institutionen,USA,Europa,Bildung,Regulierung,Content", value: "AI,Wirtschaft,Gesellschaft,Technologiewandel,Arbeitsmarkt,Produktivität,Innovation,Institutionen,USA,Europa,Bildung,Regulierung,Content", color: "hsl(18, 95%, 90%)"}
      - { label: "draft,AI,Technologie,Tools", value: "draft,AI,Technologie,Tools", color: "hsl(221, 95%, 90%)"}
      - { label: "AI,Agents,EnBW,Technologie", value: "AI,Agents,EnBW,Technologie", color: "hsl(153, 95%, 90%)"}
      - { label: "Innovation,Innovationsprozess,Templates,Produktmanagement,Unternehmensentwicklung,Methode,Tool,Skill", value: "Innovation,Innovationsprozess,Templates,Produktmanagement,Unternehmensentwicklung,Methode,Tool,Skill", color: "hsl(10, 95%, 90%)"}
      - { label: "Agents,AI,Technologie,EnBW,IBM,Meeting", value: "Agents,AI,Technologie,EnBW,IBM,Meeting", color: "hsl(8, 95%, 90%)"}
      - { label: "GitHub,Git,Gist,Repository,Skills", value: "GitHub,Git,Gist,Repository,Skills", color: "hsl(252, 95%, 90%)"}
      - { label: "Software,Kollaboration,Wissensmanagement,Git,Obsidian,Dokumentation,ITAdministration,Tool,Methode,Skill,Lösung", value: "Software,Kollaboration,Wissensmanagement,Git,Obsidian,Dokumentation,ITAdministration,Tool,Methode,Skill,Lösung", color: "hsl(210, 95%, 90%)"}
      - { label: "Methoden,Innovation,Tools", value: "Methoden,Innovation,Tools", color: "hsl(228, 95%, 90%)"}
      - { label: "Wohnen,Garten", value: "Wohnen,Garten", color: "hsl(38, 95%, 90%)"}
      - { label: "AI,Agents,Huggingface,Technologie,Automatisierung,Skill,LLM,Toolintegration,Softwareentwicklung,MachineLearning,HuggingFace,smolagents,LangGraph,LlamaIndex,Methode,Tool", value: "AI,Agents,Huggingface,Technologie,Automatisierung,Skill,LLM,Toolintegration,Softwareentwicklung,MachineLearning,HuggingFace,smolagents,LangGraph,LlamaIndex,Methode,Tool", color: "hsl(22, 95%, 90%)"}
      - { label: "GPT,Benchmark,MMLU,GPQA,AIME,SWE-Bench-Verified,Reasoning,AI,Technologie", value: "GPT,Benchmark,MMLU,GPQA,AIME,SWE-Bench-Verified,Reasoning,AI,Technologie", color: "hsl(250, 95%, 90%)"}
      - { label: "Wohnen,Smarthome,Loxone", value: "Wohnen,Smarthome,Loxone", color: "hsl(196, 95%, 90%)"}
      - { label: "AI,GPT,Reasoning,Technologie", value: "AI,GPT,Reasoning,Technologie", color: "hsl(272, 95%, 90%)"}
      - { label: "Wohnen,Pool", value: "Wohnen,Pool", color: "hsl(329, 95%, 90%)"}
      - { label: "AI,Produktentwicklung,Agenten,Innovationsmanagement,Technologieintegration,Softwareentwicklung,Digitalisierung,OpenAI,Codex,ChatGPT,Automatisierung,Content", value: "AI,Produktentwicklung,Agenten,Innovationsmanagement,Technologieintegration,Softwareentwicklung,Digitalisierung,OpenAI,Codex,ChatGPT,Automatisierung,Content", color: "hsl(239, 95%, 90%)"}
      - { label: "GitHub,Skills,Softwareentwicklung,Anleitung,Methode,Tool", value: "GitHub,Skills,Softwareentwicklung,Anleitung,Methode,Tool", color: "hsl(3, 95%, 90%)"}
      - { label: "OpenAI,AI,ChatGPT,GenAI,Perplexity,Technologie", value: "OpenAI,AI,ChatGPT,GenAI,Perplexity,Technologie", color: "hsl(40, 95%, 90%)"}
      - { label: "Infrastruktur,Softwareentwicklung,Git,DevOps,Skill,Tool,Automatisierung,Azure,VSCode,Workflow,ITAdministration,Anleitung", value: "Infrastruktur,Softwareentwicklung,Git,DevOps,Skill,Tool,Automatisierung,Azure,VSCode,Workflow,ITAdministration,Anleitung", color: "hsl(252, 95%, 90%)"}
      - { label: "UX,UI,VibeCoding,Prompting,AI,Tools,VibeDesigning,Technologie", value: "UX,UI,VibeCoding,Prompting,AI,Tools,VibeDesigning,Technologie", color: "hsl(97, 95%, 90%)"}
      - { label: "Wohnen,Heizung", value: "Wohnen,Heizung", color: "hsl(338, 95%, 90%)"}
      - { label: "AI", value: "AI", color: "hsl(137, 95%, 90%)"}
      - { label: "Klimawandel", value: "Klimawandel", color: "hsl(38, 95%, 90%)"}
      - { label: "draft", value: "draft", color: "hsl(84, 95%, 90%)"}
      - { label: "ChatGPT", value: "ChatGPT", color: "hsl(213, 95%, 90%)"}
      - { label: "Perplexity", value: "Perplexity", color: "hsl(129, 95%, 90%)"}
      - { label: "GPT", value: "GPT", color: "hsl(241, 95%, 90%)"}
      - { label: "Reasoning", value: "Reasoning", color: "hsl(171, 95%, 90%)"}
      - { label: "OpenAI", value: "OpenAI", color: "hsl(146, 95%, 90%)"}
      - { label: "Prompting", value: "Prompting", color: "hsl(3, 95%, 90%)"}
      - { label: "Technologie", value: "Technologie", color: "hsl(25, 95%, 90%)"}
      - { label: "Agents", value: "Agents", color: "hsl(224, 95%, 90%)"}
      - { label: "Digitalisierung", value: "Digitalisierung", color: "hsl(198, 95%, 90%)"}
      - { label: "Energiewirtschaft", value: "Energiewirtschaft", color: "hsl(164, 95%, 90%)"}
      - { label: "Datenökosysteme", value: "Datenökosysteme", color: "hsl(326, 95%, 90%)"}
      - { label: "Energiedatenräume", value: "Energiedatenräume", color: "hsl(106, 95%, 90%)"}
      - { label: "Gaia-X", value: "Gaia-X", color: "hsl(199, 95%, 90%)"}
      - { label: "IT-Architektur", value: "IT-Architektur", color: "hsl(9, 95%, 90%)"}
      - { label: "energydata-X", value: "energydata-X", color: "hsl(216, 95%, 90%)"}
      - { label: "EnBW", value: "EnBW", color: "hsl(141, 95%, 90%)"}
      - { label: "Initiative", value: "Initiative", color: "hsl(63, 95%, 90%)"}
      - { label: "These", value: "These", color: "hsl(277, 95%, 90%)"}
      - { label: "Blockchain", value: "Blockchain", color: "hsl(158, 95%, 90%)"}
      - { label: "Anthropic", value: "Anthropic", color: "hsl(261, 95%, 90%)"}
      - { label: "Softwareentwicklung", value: "Softwareentwicklung", color: "hsl(35, 95%, 90%)"}
      - { label: "Automatisierung", value: "Automatisierung", color: "hsl(353, 95%, 90%)"}
      - { label: "Agenten", value: "Agenten", color: "hsl(200, 95%, 90%)"}
      - { label: "Entwicklerproduktivität", value: "Entwicklerproduktivität", color: "hsl(49, 95%, 90%)"}
      - { label: "Infrastruktur", value: "Infrastruktur", color: "hsl(318, 95%, 90%)"}
      - { label: "Cloud", value: "Cloud", color: "hsl(21, 95%, 90%)"}
      - { label: "GitHub", value: "GitHub", color: "hsl(311, 95%, 90%)"}
      - { label: "Copilot", value: "Copilot", color: "hsl(52, 95%, 90%)"}
      - { label: "Microsoft", value: "Microsoft", color: "hsl(77, 95%, 90%)"}
      - { label: "Arbeitswelt", value: "Arbeitswelt", color: "hsl(131, 95%, 90%)"}
      - { label: "Produktivität", value: "Produktivität", color: "hsl(321, 95%, 90%)"}
      - { label: "OpenSource", value: "OpenSource", color: "hsl(108, 95%, 90%)"}
      - { label: "Coding", value: "Coding", color: "hsl(281, 95%, 90%)"}
      - { label: "Content", value: "Content", color: "hsl(120, 95%, 90%)"}
      - { label: "Wirtschaft", value: "Wirtschaft", color: "hsl(56, 95%, 90%)"}
      - { label: "Gesellschaft", value: "Gesellschaft", color: "hsl(24, 95%, 90%)"}
      - { label: "Technologiewandel", value: "Technologiewandel", color: "hsl(178, 95%, 90%)"}
      - { label: "Arbeitsmarkt", value: "Arbeitsmarkt", color: "hsl(59, 95%, 90%)"}
      - { label: "Innovation", value: "Innovation", color: "hsl(302, 95%, 90%)"}
      - { label: "Institutionen", value: "Institutionen", color: "hsl(104, 95%, 90%)"}
      - { label: "USA", value: "USA", color: "hsl(132, 95%, 90%)"}
      - { label: "Europa", value: "Europa", color: "hsl(54, 95%, 90%)"}
      - { label: "Bildung", value: "Bildung", color: "hsl(19, 95%, 90%)"}
      - { label: "Regulierung", value: "Regulierung", color: "hsl(285, 95%, 90%)"}
      - { label: "Tools", value: "Tools", color: "hsl(32, 95%, 90%)"}
      - { label: "Innovationsprozess", value: "Innovationsprozess", color: "hsl(329, 95%, 90%)"}
      - { label: "Templates", value: "Templates", color: "hsl(329, 95%, 90%)"}
      - { label: "Produktmanagement", value: "Produktmanagement", color: "hsl(123, 95%, 90%)"}
      - { label: "Unternehmensentwicklung", value: "Unternehmensentwicklung", color: "hsl(242, 95%, 90%)"}
      - { label: "Methode", value: "Methode", color: "hsl(336, 95%, 90%)"}
      - { label: "Tool", value: "Tool", color: "hsl(25, 95%, 90%)"}
      - { label: "Skill", value: "Skill", color: "hsl(38, 95%, 90%)"}
      - { label: "IBM", value: "IBM", color: "hsl(269, 95%, 90%)"}
      - { label: "Meeting", value: "Meeting", color: "hsl(195, 95%, 90%)"}
      - { label: "Git", value: "Git", color: "hsl(63, 95%, 90%)"}
      - { label: "Gist", value: "Gist", color: "hsl(155, 95%, 90%)"}
      - { label: "Repository", value: "Repository", color: "hsl(67, 95%, 90%)"}
      - { label: "Skills", value: "Skills", color: "hsl(169, 95%, 90%)"}
      - { label: "Software", value: "Software", color: "hsl(33, 95%, 90%)"}
      - { label: "Kollaboration", value: "Kollaboration", color: "hsl(61, 95%, 90%)"}
      - { label: "Wissensmanagement", value: "Wissensmanagement", color: "hsl(24, 95%, 90%)"}
      - { label: "Obsidian", value: "Obsidian", color: "hsl(329, 95%, 90%)"}
      - { label: "Dokumentation", value: "Dokumentation", color: "hsl(345, 95%, 90%)"}
      - { label: "ITAdministration", value: "ITAdministration", color: "hsl(48, 95%, 90%)"}
      - { label: "Lösung", value: "Lösung", color: "hsl(195, 95%, 90%)"}
      - { label: "Methoden", value: "Methoden", color: "hsl(70, 95%, 90%)"}
      - { label: "Wohnen", value: "Wohnen", color: "hsl(93, 95%, 90%)"}
      - { label: "Garten", value: "Garten", color: "hsl(280, 95%, 90%)"}
      - { label: "Huggingface", value: "Huggingface", color: "hsl(151, 95%, 90%)"}
      - { label: "LLM", value: "LLM", color: "hsl(188, 95%, 90%)"}
      - { label: "Toolintegration", value: "Toolintegration", color: "hsl(125, 95%, 90%)"}
      - { label: "MachineLearning", value: "MachineLearning", color: "hsl(197, 95%, 90%)"}
      - { label: "HuggingFace", value: "HuggingFace", color: "hsl(202, 95%, 90%)"}
      - { label: "smolagents", value: "smolagents", color: "hsl(60, 95%, 90%)"}
      - { label: "LangGraph", value: "LangGraph", color: "hsl(313, 95%, 90%)"}
      - { label: "LlamaIndex", value: "LlamaIndex", color: "hsl(350, 95%, 90%)"}
      - { label: "Benchmark", value: "Benchmark", color: "hsl(126, 95%, 90%)"}
      - { label: "MMLU", value: "MMLU", color: "hsl(1, 95%, 90%)"}
      - { label: "GPQA", value: "GPQA", color: "hsl(37, 95%, 90%)"}
      - { label: "AIME", value: "AIME", color: "hsl(9, 95%, 90%)"}
      - { label: "SWE-Bench-Verified", value: "SWE-Bench-Verified", color: "hsl(13, 95%, 90%)"}
      - { label: "Smarthome", value: "Smarthome", color: "hsl(133, 95%, 90%)"}
      - { label: "Loxone", value: "Loxone", color: "hsl(9, 95%, 90%)"}
      - { label: "Pool", value: "Pool", color: "hsl(90, 95%, 90%)"}
      - { label: "Produktentwicklung", value: "Produktentwicklung", color: "hsl(102, 95%, 90%)"}
      - { label: "Innovationsmanagement", value: "Innovationsmanagement", color: "hsl(197, 95%, 90%)"}
      - { label: "Technologieintegration", value: "Technologieintegration", color: "hsl(234, 95%, 90%)"}
      - { label: "Codex", value: "Codex", color: "hsl(198, 95%, 90%)"}
      - { label: "Anleitung", value: "Anleitung", color: "hsl(255, 95%, 90%)"}
      - { label: "GenAI", value: "GenAI", color: "hsl(297, 95%, 90%)"}
      - { label: "DevOps", value: "DevOps", color: "hsl(199, 95%, 90%)"}
      - { label: "Azure", value: "Azure", color: "hsl(194, 95%, 90%)"}
      - { label: "VSCode", value: "VSCode", color: "hsl(190, 95%, 90%)"}
      - { label: "Workflow", value: "Workflow", color: "hsl(56, 95%, 90%)"}
      - { label: "UX", value: "UX", color: "hsl(199, 95%, 90%)"}
      - { label: "UI", value: "UI", color: "hsl(133, 95%, 90%)"}
      - { label: "VibeCoding", value: "VibeCoding", color: "hsl(228, 95%, 90%)"}
      - { label: "VibeDesigning", value: "VibeDesigning", color: "hsl(223, 95%, 90%)"}
      - { label: "Heizung", value: "Heizung", color: "hsl(297, 95%, 90%)"}
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: true
      task_hide_completed: true
      footer_type: none
      persist_changes: false
      content_alignment: text-align-left
  __created__:
    key: __created__
    id: __created__
    input: metadata_time
    label: Created
    accessorKey: __created__
    isMetadata: true
    isDragDisabled: false
    skipPersist: false
    csvCandidate: true
    position: 3
    width: 160
    isHidden: true
    sortIndex: -1
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
config:
  remove_field_when_delete_column: false
  cell_size: compact
  sticky_first_column: true
  group_folder_column: 
  remove_empty_folders: false
  automatically_group_files: false
  hoist_files_with_empty_attributes: true
  show_metadata_created: true
  show_metadata_modified: false
  show_metadata_tasks: false
  show_metadata_inlinks: false
  show_metadata_outlinks: false
  show_metadata_tags: false
  source_data: current_folder
  source_form_result: 
  source_destination_path: /
  row_templates_folder: /
  current_row_template: 
  pagination_size: 200
  font_size: 12
  enable_js_formulas: false
  formula_folder_path: /
  inline_default: false
  inline_new_position: last_field
  date_format: dd.MM.yyyy
  datetime_format: "dd.MM.yyyy HH:mm:ss"
  metadata_date_format: "dd.MM.yyyy HH:mm:ss"
  enable_footer: false
  implementation: default
filters:
  enabled: true
  conditions:
      - condition: OR
        disabled: true
        label: "Blockchain"
        color: "hsl(200, 95%, 90%)"
        filters:
        - field: tags
          operator: CONTAINS
          value: "DLT"
          type: tags
        - field: tags
          operator: CONTAINS
          value: "Blockchain"
          type: tags
      - condition: OR
        disabled: true
        label: "AI"
        color: "hsl(284, 95%, 90%)"
        filters:
        - field: tags
          operator: CONTAINS
          value: "AI"
          type: tags
        - field: tags
          operator: CONTAINS
          value: "KI"
          type: tags
      - condition: OR
        disabled: true
        label: "Meetings"
        color: "hsl(69, 95%, 90%)"
        filters:
        - field: tags
          operator: CONTAINS
          value: "Meeting"
          type: tags
```