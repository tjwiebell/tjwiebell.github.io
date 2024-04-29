# State of Accessibility - GivePulse 2024

Building upon the [Accessibility Roadmap][1] created in 2022, this document will highlight improvements made in 2023, and a roadmap of proactive changes for 2024 we plan to incrementally roll out. Before any commitments are made, or blogs are published, we should message this as a subject of constant evolution, and without broad education in these topics, we're only as good as the published content we allow on our platform.

## 2022 Health Check

Quick review of the previous document, and how we did hitting those goals.

| Objective | Result |
| --------- | ------ |
| Drag and Drop Keyboard Support | 🟡 Still using the same classic builder
| Navigation Shortcuts | 🟢 Two _Jump to Content_ elements added
| Labels and Descriptions | 🟡 One of those constant improvement areas, but good chunk of effort started here
| Buttons vs. Links | 🟡 Still some tech debt, but lint rules in ensure anything routeable is a semantic link `<a>`
| iOS and Android | 📌 React Native should handle this, but bad semantics could still lead to similar problems in the web app; should follow-up
| Loose QA Note | A version of this _Additional Information_ statement can come over, but not much of this is in place yet

## April 2023 - The Awakening

A frontend engineer with contributions to `@adobe/react-aria` joins the company, who tries and mostly fails to help improve things in the immediate. A regular meeting cadence was maintained, and we still accomplished a great deal without any clear objectives outside of our goal to deliver as much value in what we did focus on.

| Improvement | Notes |
| ----------- | ----- |
| Event Creation | First area of focus, was able to add some focus management, label/help text improvements, required indicators, but changes were risky
| Training | Weekly meetings with engineers to discuss a11y review comments, and education on web semantics
| Dashboard | This might be a bold assumption, but I believe Dashboard is the first new feature I would be confident passes 2.1 AA standards
| Storybook | Isolated sandbox, easier to introduce fixes while ensuring no regressions. A11y plugin automatically tests all components and reports warnings and errors based on different guidelines.
| Theme Refresh | Directly working with Seulki to align the theme the developers are using the build components with the one in Figma. Color constrast is now calculated at build time, and guaranteed to meet minimum guidelines. Response font sizing added. Visual regression 🤞
| Automated Testing | Accessible markup is required for test actions, two for one checks
| Tools | Using the identical aXe tooling that 80% of the screen reader market; less guess work that our _fix_ does what we intend

## April 2024 - Ziggurat

Looking forward, an unprioritized list of improvements we could focus on for the next 1+ years.

- Visual Regression Tests
- Measurement of Success
- Automated a11y Checks
- Full Page aXe Reports
- Internal Training
- Content Creator Guidance and Documentation
- Accessible Bug Reporting and Bounty Credit

[1]: (https://drive.google.com/file/d/1-VDqc3TN-Qu1smzqZ_HokQhU2q5Bwb53/view?usp=sharing)
