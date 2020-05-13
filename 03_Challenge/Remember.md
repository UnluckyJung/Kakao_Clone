# :notebook: 애 먹었던점

## :question: 색깔

* 문제에서 요구하는 색이 무슨색인지 몰랐었다.
* :heavy_check_mark: 그림판을 이용해서 `rgb`값을 따서 해결했다.

## :question: Red-box `Fix`

### 고정이 안되었다.
* `fixed`후 `top` 같은 기준 값을 정해주지 않았던것이 원인이었다.
*  :heavy_check_mark: `top : 0px`를 주어 해결했다.

### 고정후에 이상하게 배치되었다.
* `postion`에 `fixed`를 주면 레이아웃을 아예 무시하고 크기가 고정 되던게 원인이었다.
* 즉 `display : block;` 이 무시 되었다.
* :heavy_check_mark: 가짜 `box`를 만들고 `block` 옵션을 주었다.

## :question: Yellow box `inline-block 공백`
* `inline-block` 간에 자꾸 공백이 생겼었다.
* :heavy_check_mark: 여러가지 해결방법이 있지만, 나는 `float` 을 이용해 해결하였다.
* :heavy_check_mark: `float : right;`

## :question: Yellow box bounder 굵기로 인한 `크기 확장 = 레이아웃 파괴`
* `bounder` 에 크기를 주니 커져서 자꾸 레이아웃이 망가졌다.
* :heavy_check_mark: `box-sizing` 를 이용해 해결했다. 
    * 크기가 켜져도 `border box` 크기에 맞춰 비율을 조절해준다.
* :heavy_check_mark: `box-sizing: border-box;`

## :question: Green box `size`
* 브라우저 크기에 따라서 `Green box`가 유동적으로 움직이지 않았다.
* :heavy_check_mark: `body`에 `relation`을 주고 `green box`에 `absolute`로 의존성을 걸어 해결했다.

---