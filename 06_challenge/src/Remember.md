# :book: 기억할점

### :heavy_check_mark: 원을 만드는법
* `height`와 `width`를 같게 준다
* `border-radius`를 절반으로 준다.

```css
.circle {
  background-color: white;
  width: 20px;
  height: 20px;
  border-radius: 10px;
}
```

### :heavy_check_mark: 애니메이션 딜레이주기
* `속도 뒤`에 붙여준다.
```css
.sample{
  animation: "keyframename" "속도" "딜레이" "효과";
}
```

### :heavy_check_mark: 애니메이션 끝내고 대기시키기
* `100% 전에` none을 주고, 그 뒤에 아무것도 주지않는다.

```css
@keyframes StickSize {
  0% {
    transform: none;
  }
  15% {
    transform: scale(1, 2);
  }
  30% {
    transform: none;
  }
}
```
