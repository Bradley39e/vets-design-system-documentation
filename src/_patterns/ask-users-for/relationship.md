---
layout: pattern
permalink: /patterns/ask-users-for/relationship
sub-section: ask-users-for
title: Relationship to Veteran
intro-text: "Follow this pattern to ask a user for their relationship to the Veteran."
code-link: https://github.com/department-of-veterans-affairs/vets-website/blob/main/src/platform/forms-system/src/js/web-component-patterns/relationshipToVeteranPattern.jsx
example-link: https://staging.va.gov/mock-form-patterns/relationship-to-veteran
github-title: pattern-relationship-to-veteran
research-title: Ask users for relationship to Veteran
sketch-link: https://www.sketch.com/s/dc844743-277e-41d4-81ba-a48fd0743952/p/CDC8B63A-CD03-4A68-8130-9F2A106D0961/canvas
status: use-deployed
anchors:
  - anchor: Usage
  - anchor: Examples
  - anchor: How to design and build
  - anchor: Content considerations
---

## Usage

### When to use this pattern

* **Asking for the relationship to the Veteran.** For example, when a caregiver is filling out a form.
 
## Examples

### Relationship to Veteran

{% include component-example.html alt="An example of asking the relationship to the Veteran with radio buttons." file="/images/patterns/ask-users-for/relationship/relationship-to-veteran.png" caption="Example of asking the relationship to the Veteran with radio buttons." width="50%" %}

<a class="vads-c-action-link--blue" href="{{ page.example-link }}">
  View an example
  
## How to design and build 

### How this pattern works

- **Use either a drop down or radio buttons.** Options should include spouse, child, parent, executor/administrator of estate or other.
- **Provide a way to give a ‘None of the above’ answer.** A radio button labeled “Other” should be provided.

#### Conditionally revealed fields can be used if the following conditions are met:
1. There should only be one reveal on a page.
2. When the revealed trigger is selected, you must be able to tab directly into the newly revealed field. (which is why we've put the "other" question last.)
3. The newly revealed question field must be understood by itself.  For example, don't just say "Other". Say, "Since your relationship with the veteran was not listed, please describe it here"

{% include component-example.html alt="An example of a conditionally revealed field" file="/images/patterns/ask-users-for/relationship/relationship-to-veteran-other.png" caption="Example of asking the relationship to the Veteran with radio buttons and a conditionally revealed field." width="50%" %}



### Error message templates for addresses

**When a user doesn’t select a relationship:**

Say "Select your relationship to the Veteran"
