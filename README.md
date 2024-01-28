# Refactoring dy-mde

### What are we currently dealing with?
---
Started back in **Feb 2021**, as a successor of mobile-app, dy-mde has spiralled into a complex, challenging and a difficult to read, maintain and debug repository which needs a serious overhaul in terms of code, also known as refactoring. By adopting an approach of getting stuff shipped fast, we've compromised on a lot of fundamental measures like writing unit tests, using a ReactJS framework, using TypeScript, so on and so forth. We even lack the most basic eslint.

### Pain points
--- 
From having large components to not adhering to principles like DRY (Don't Repeat Yourself), KISS(Keep It Simple Silly) and separation of concerns, we have quite a long list of problems on our hands which need to be tackled in a way that it not only improves the DX (Developer Experience) but also brings in consistency across the entire repository