# React

## Tech Stack ( Ecosystem )

**Server:** Node, Express, NextJS

**UI Framework:** Ant Design, Material UI

**CSS Framework:** TailwindCSS, Bulma, Bootstrap (v5)

**CSS Preprocessor:** SASS/SCSS

**State management:** Redux, Redux toolkit (Flux concept)

**Side effect:** React-query, Saga, Redux thunk




## Used By

This project is used by the following companies:

- Có bao nhiêu Hook trong React
***Có hơn 10 hooks ***

***ex: useState, useCallback, useMemo, useEffect, useLayoutEffect, useRef, useReducer, useImperativehandle, useContext, useDebugValue***

- useRef thì có khác gì với useState
***useRef không có function để render lại UI***

***useState có setState để làm render lại UI.***

***useRef để gắn pointer đến element của HTML hoặc để lưu temp***

- Khác nhau props và state
***Props: là định nghĩa data được nhận từ bên ngoài component.***

***State: là định nghĩa data đang lưu trữ trong component***

- So sánh class và hook

***Class: Triển khai theo dạng OOP Class, luôn return về JSX Element*** 

***Hook: Triển khai theo dang Function, return về đa dạng value, có tính reuseable và scaleable từ các custom-hook***


- So sánh Component và PureComponent
***Trong Life Cycle PureComponent sẽ chạy vào shouldComponentUpdate shallow compare object Props, Class Component thì không ***

- Life Cycle Class Component
```
3 Trạng thái: Mount, UpdateMount, UnMount
Các function được thực hiện theo thứ tự từ trái sang phải.
Mount: Contructor -> Willmount -> Render -> Didmount
UpdateMount: getDerivedStateFromProps -> shouldComponentUpdate -> render -> componentDidUpdate.
UnMount: componentWillUnmount
```

- Life Cycle Hook
```
Contructor -> useLayoutEffect -> render -> useEffect
```
- Virtual DOM
***Tốc độ không nhanh hơn RealDOM, Virtual DOM giúp cho thuật toán của React không render lại UI dư thừa***

- One way binding
***Luồng dữ liệu 1 chiều như LifeCycle React hoạt động, giúp cho quá trình kiểm tra các issue trở nên dễ dàng hơn***

- So sánh useCallback và useMemo
***Đều là CACHE useCallBack sẽ return về 1 function và có tham số nếu function có định nghĩa, useMemo sẽ return về 1 value***

- So sánh useMemo và reactMemo
***useMemo là cache bên trong Component, React Memo Cache bên ngoài Component***

- So sánh uselayouteffect và useeffect
***Theo LifeCycle uselayouteffect sẽ render trước useeffect***

- Nên đặt side effect (call api) ở đâu?
***Class Component thì đặt ở Didmount, Hook thì đặt ở useEffect***
***Đặt trước khi render được không (Willmount, useLayoutEffect) -> Được***

- Tạo sao nên đặt key trong component
***Virtual DOM được định danh bằng Key, Không đặt Key sẽ gây ra lỗi Render UI nếu có 2 component giống nhau render 1 danh sách giống nhau trong 1 component***

- Phân biệt server side và client side
***Render HTML ở server tốt cho SEO, nhưng không tốt cho UX***
***Đưa HTML, CSS, JS về cho browser xử lý, Tốt cho UX nhưng không tốt cho SEO***

- Unit Test
***Dùng Jest để xử lý unit test ( snappsot và test cases api )***

- Phân biệt composition và inherit
***Inherit không có tính reuseable cao như composition***

