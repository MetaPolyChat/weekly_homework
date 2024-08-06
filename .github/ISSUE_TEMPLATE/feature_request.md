---
name: Feature request
about: Suggest an Feature
title: Add new Feature
labels: ''
assignees: ''

---

name: "Add Feature"
description: "기능에 대한 설명"
title: "[Feat]: "
labels: ["feature"]
assignees:
  - writeYourName
body:
  - type: markdown
    attributes:
      value: |
        Please check new feature
  - type: input
    id: input_name
    attributes:
      label: 기능명
      description: 기능을 설명해주세요
      placeholder: 기능 설명 작성
    validations:
      required: true
