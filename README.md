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

#### 문제. 확장된/조합된 컴포넌트를 정의할 때 커스텀 엘리먼트를 createElement로 생성하면 조합 컴포넌트 스콥의 스타일을 상속할 수 없다. slot은 너무 유연해지는데, class 를 확장해야 하는지

#### aria-selected 등 aria 속성을 스타일링을 위해 상속할 때 커스텀 엘리먼트에서 selected 로 요약해서 작성하지 않고 aria-selected 그대로 사용하는 것이 좋겠다.
