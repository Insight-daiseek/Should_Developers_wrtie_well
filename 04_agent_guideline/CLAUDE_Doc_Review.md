# Document Review Workflow

Apply this workflow when reviewing, writing, or revising documentation in this repository. It is for developers and coding agents responsible for documentation. Its goal is to help readers find accurate information easily while preserving the source document's facts and technical meaning.

## 1. Confirm the task before starting

1. Resolve every relative path from the repository root that contains this file.
2. Confirm the task scope: target document, task purpose, document type, and whether source edits are allowed.
3. When the document type is not specified, determine how the reader will use it. If there is not enough evidence, do not edit based on an assumption; report `확인 필요` (confirmation needed).
4. Distinguish the requested work:
   - **Review**: report issues and proposed changes only; do not edit the source.
   - **Revision**: edit the source against the applicable checklists.
   - **Saved review report**: save the review results as a separate Markdown file.

## 2. Select and read the checklists

For every task, read and apply these shared checklists in order:

1. `02_checklists/00_common/01_common_quality.md`
2. `02_checklists/00_common/02_reader_and_topic.md`
3. `02_checklists/00_common/03_outline.md`

Then select the reading mode.

- **Reference document**: readers look up specific information. This includes manuals, procedures, functional specifications, and project READMEs.
- **Reading document**: readers follow the document from beginning to end. This includes development reports, proposals, and technical blogs.
- If the mode cannot be determined, do not guess; report `확인 필요`.

### Reference document

Also read the base checklist and one matching detail checklist:

1. `02_checklists/10_reference_documents/10_reference_base.md`
2. Detail type
   - Product manual: `11_product_manual.md`
   - Feature manual: `12_feature_manual.md`
   - Procedure: `13_procedure.md`
   - External functional specification: `14_external_function_spec.md`
   - Implementation specification: `15_implementation_spec.md`
   - Project README: `17_project_readme.md`

All detail files are in `02_checklists/10_reference_documents/`.

### Reading document

Also read the base checklist and one matching detail checklist:

1. `02_checklists/20_reading_documents/20_reading_base.md`
2. Detail type
   - Development report: `21_development_report.md`
   - Model development report: apply `21_development_report.md` first, then `24_model_development_report.md`
   - Product proposal: `22_product_proposal.md`
   - Technical blog: `23_technical_blog.md`

All detail files are in `02_checklists/20_reading_documents/`.

## 3. Review and revise

1. Identify the document's readers, reader goal, scope, and type.
2. Compare the source against every item in the selected checklists.
3. For every finding, record the location, checklist basis, issue, and revision direction.
4. For a revision task, edit only within the evidence-supported scope. When changing structure, also check headings and cross-references.
5. After revision, read only the title and headings once to verify information location and logical flow.

Follow these rules throughout the work:

- Do not add, remove, or change facts, numbers, policies, technical behavior, or intent without evidence.
- Put unsupported or ambiguous content in `확인 필요`; do not silently make it more specific.
- If checklist items conflict or applicability is unclear, do not decide arbitrarily. Report `확인 필요` with the reason.
- Do not edit the source for a review-only task. Edit only when the user explicitly requests or permits revision.
- Ask the user before fact-checking external sources, changing policy, or taking an action that is hard to reverse or affects other documents or systems.

## 4. Deliverables and completion

Lead the final result with the outcome and include:

- document type and checklist files applied;
- key findings or changes made;
- `확인 필요` items and their reasons, or state that there are none;
- whether the source was edited and which files changed.

If the user asks to save a review report as Markdown, first read `03_docs_template/01_agent/document-review-report-template.md` and follow its format. Replace or remove template guidance and example rows with the actual result. Omit `제안 구조` when no structural change is necessary.

The task is complete only when all selected checklists were applied, review and revision boundaries were preserved, headings were validated, and every required confirmation was reported.
