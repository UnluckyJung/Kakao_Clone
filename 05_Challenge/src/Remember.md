# :book: 기억할점

### :pencil: 이미지 첨부하기
> :heavy_check_mark: `img 태그 src = "이미지주소"`

* `src`에 이미지 주소를 넣는다.
* `크기`는 `html`에서 바로 설정해도 되고, `css`에서 설정해도 된다.
* `alt`는 대체 이미지를 넣는곳이다. `텍스트`도 가능하다.

```html
    <img
      class="이미지 이름"
      src="이미지 주소"
      alt="대체 텍스트나 이미지"
    />
```


### :pencil: 모서리를 둥글게하기
> :heavy_check_mark: `border-radius"`

* 모서리를 둥글게한다.
* 둥글게하며 삐져 나오는게 있기 때문에 `border` 크기를 `0`으로 바꿔준다.

```css
button{
  border: 0px;
  border-radius: 40px;
}
```

### :pencil: 그림자 효과주기
> :heavy_check_mark: `box-shadow: "x방향" "y방향" "정도" "색";`

```css
.box{
  box-shadow: 0px 0px 10px grey;
}
```

### :pencil: 글씨를 창크기에 맞춰 유동적으로 변하게 하기
> :heavy_check_mark: `vw` `vh` `vmin` `vmax` 단위를 쓴다. 

* 너비, 높이, 둘중 작은것, 둘중 큰것을 기준으로 잡아 유동적으로 글씨 크기가 변한다.
```css
.button{
  font-size: 4vw;
}
```

---

## :heavy_exclamation_mark: 기억 못한것
* `flex`의 모든 설정은 `부모`에서 한다.
