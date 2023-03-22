# Improve-performance-reactjs
- Khi code 1 UI có những component không cần thiết phải render lại mỗi khi state thay đổi
- Ví dụ: Button gọi 1 hành động, Image tĩnh ... 

## Redux
![example-useSelector](https://user-images.githubusercontent.com/62127758/226834412-aa968a97-5b80-4e70-a979-9fe8a1d11801.png)<br />
![example-mapStateToProps](https://user-images.githubusercontent.com/62127758/226836346-fa9431ca-6690-4d21-8604-b2b90d50f8d0.png)
- Sử dụng hooks `useMemo()` hoặc HOC `memo()` của react
- Khi global state thay đổi, tất cả sẽ re-render => Get chính xác state cần sử dụng
![solution-useSelector](https://user-images.githubusercontent.com/62127758/226837188-9b71529a-10f6-4d6f-8879-8967db4f659d.png)<br />
![solution-mapStateToProps](https://user-images.githubusercontent.com/62127758/226837026-996cb8e2-a387-49f6-8279-4ec005d05faa.png)
- Mọi thứ sẽ ok khi sử dụng `mapStateToProps` trong `connect` của react redux.



