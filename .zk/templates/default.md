---
id: {{id}}
date: {{date now "%Y-%m-%d %H:%M:%S%z"}}
title: {{json title}}
{{#each extra}}
{{@key}}: {{json this}}
{{/each}}
---

{{content}}
