# AI-Assisted Workflow Drill

## Feature

For this exercise, I built the same student account settings form twice using AI. Both versions used HTML and CSS, but I deliberately changed the quality of the instructions given to Claude.

## Round One: Vague Prompt

For the first version, I gave Claude a short and vague request to create a student account settings form with validation. I intentionally provided very little information about accessibility, responsive behavior, validation rules, visual requirements, or implementation constraints.

Claude was able to produce a usable starting point quickly, but the lack of specification meant that I had to rely on the model's assumptions. Important implementation decisions were not explicitly controlled by me.

## Round Two: Structured Prompt

For the second version, I started a fresh Claude conversation and provided a detailed specification. I defined the required fields, HTML validation requirements, accessibility expectations, responsive behavior, technology constraints, and expected output format. I also asked Claude to plan before coding and verify the result against the requirements afterward.

This produced a more deliberate implementation because Claude had clear criteria against which its own output could be reviewed.

## Comparison

The biggest difference was not simply visual quality but predictability. In round one, Claude decided many requirements for itself. In round two, requirements such as associated labels, semantic HTML, keyboard focus states, responsive layout, required fields, email validation, and password length were explicitly defined.

The structured workflow also made edge cases easier to identify. One important limitation was password-confirmation validation. HTML and CSS alone cannot reliably compare two password values. A structured verification step should acknowledge this limitation rather than pretending the requirement is fully implemented.

## What I Learned

The experiment showed me that AI-generated code still requires engineering direction and review. A vague prompt can generate code quickly, but a precise specification reduces assumptions and makes verification easier. For future features, I will define constraints, accessibility requirements, edge cases, and verification criteria before asking AI to implement them.
