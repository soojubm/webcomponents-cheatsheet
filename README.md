# webcomponents-cheatsheet

#### component tokens usage
- dataset으로 스타일링 하지 않기
- 모든 프로젝트와 모든 컴포넌트에 aria가 정의되어 있다면 조금 고민이 됨
```
:host {
  --chip-color-background: var(--color-background-weak);
  --chip-color-border: var(--color-border);
}
:host([status=info]) {
  --chip-color-background: var(--color-status-info);
  --chip-color-border: transparent;
}
```
