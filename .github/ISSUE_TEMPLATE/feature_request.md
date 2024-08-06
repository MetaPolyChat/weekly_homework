---
name: Feature request
about: Suggest an Feature
title: Add new Feature
labels: ''
assignees: ''

---

name: "기능명"
description: "기능에 대한 설명"
title: "이슈 제목"
labels: ["태그"]
assignees:
  - writeYourName
body:
  - type: markdown
    attributes:
      value: |
        # 기능 테스트

        report page image

        ## 메서드 설명
  - type: input
    id: input_name
    attributes:
      label: 📣 기능 이름
      description: 💭 기능의 이름을 작성해 주세요
      placeholder: 🫧 <이름>
    validations:
      required: true
  - type: textarea
    id: textarea_description
    attributes:
      label: 📣 기능 추가 이유
      description: 💭 기능 추가하는 이유을 적어주세요
      placeholder: |
        🫧 <기능 생성 이유>
        1. <이유>
        2. <이유>
      render: ''
    validations:
      required: true
  - type: textarea
    id: textarea_work
    attributes:
      label: ✅ 작업 리스트
      description: 💭 작업에 필요한 목록 작성
      placeholder: |
        🫧 <ex. 예시 지문>
        - [ ] <체크 1>
        - [ ] <체크 2>
      value: |
        - [ ] <작업 1>
        - [ ] <작업 2>
        - [ ] <작업 3>
        - [ ] 더입력 ...
      render: ''
    validations:
      required: true
  - type: checkboxes
    id: checkboxes_list
    attributes:
      label: 📣 작성자 체크리스트
      description: 💭 작성자 체크리스트
      options:
        - label: 🔱 기능 제목을 적절하게 정하였습니까?
          required: false
        - label: 🔱 작업 리스트를 이슈에 맞게 설정하셨습니까?
          required: false
        - label: 📍 타이틀에 기능 이름을 추가하였습니까?
          required: true
        - label: 📌 작성자는 모든 작업에 대한 정보가 공개됨을 동의함니까?
          required: true
