
#### useAliasesForRenames

F2 버튼을 사용해 변수 이름을 변경할 때, javascript(typescript) 인 경우 이름이 변경되는 것이 아니라, 변수의 별칭을 설정한다.

이것이 불편한 경우 아래 두 값을 `false` 로 설정한다.

`typescript.preferences.useAliasesForRenames`
`javascript.preferences.useAliasesForRenames`

설정 예시 :
```
{
  "typescript.preferences.useAliasesForRenames": false,
  "javascript.preferences.useAliasesForRenames": false
}
```


#### jest.runMode

`on-demand` : UI 에서 수동으로 실행하려는 경우 설정한다.

설정 예시 :
```
{
  "jest.runMode": "on-demand"
}
```
