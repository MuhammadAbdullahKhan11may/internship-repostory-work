
# Project AI Development Rules

These rules were established after comparing a vague AI coding prompt with a structured implementation workflow.

## Rule 1: Accessible Form Controls

Every form input must have a clearly associated label. Form controls must also provide visible keyboard focus states and must not rely only on color to communicate important information.

## Rule 2: Define Validation Before Implementation

Before generating a form, required fields and validation behavior must be explicitly defined. Appropriate HTML input types and built-in validation attributes should be used whenever possible.

## Rule 3: Respect Technology Limitations

Do not claim that a requirement has been implemented when the selected technologies cannot support it. For example, HTML and CSS alone cannot reliably validate that two password fields contain matching values.

## Rule 4: Keep Changes Within Scope

Do not introduce frameworks, libraries, JavaScript, or unrelated changes unless they are explicitly required by the feature specification.

## Rule 5: Verify Against Requirements

After generating code, review the implementation against every stated requirement and identify anything that is missing, partially implemented, or impossible with the current technology.
