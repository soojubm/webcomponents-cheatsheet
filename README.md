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


#### slot
- react의 children 맥락으로 사용
- 모든 edge case를 컴포넌트 정의할 필요가 없고ㅡ다시 말해서 props에서 정의할 필요가 없다. 세부사항과 세부사항의 조합을 위시하는 패턴 정의가 더욱 중요.


#### host element?는 inline display가 기본값. 상하 간격에 주의.
