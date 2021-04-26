flex có 2 thuộc tính là:
- main chiều ngang
- cross chiều dọc

flex container:
- display: flex
- flex-direction:
    + row: các element sẽ nằm từ trái sang phải theo chiều ngang
    + column: các element sẽ nằm từ trên xuống dưới theo chiều dọc
    + column-reverse: các element sẽ nằm từ dưới lên trên theo chiều dọc
    + row-reverse: các element sẽ nằm từ phải sang trái theo chiều ngang

- flex-wrap:
    + nowrap: các flex nằm theo chiều ngang và tràn nếu dài hơn chiều dài container
    + wrap:  các flex nằm theo chiều ngang và xuống dòng nếu dài hơn chiều dài container

- flex-flow: (Viết tắt của flex-direction và flex-wrap)
    + row wrap

- justify-content:
    + flex-start: các item bắt đàu từ trái sang phải
    + flex-end: <nt ngược lại>
    + center: ở giữa
    + space-between: cách đều  các element
    + space-around: ở 2 element giữa và cuối có khoảng trắng
    + space-evenly: ở 2 element giữa và cuối có khoảng trắng nhưng bằng nhau

- align-items:
    + center: căn giữa theo chiều cross
    + flex-end: dưới cùng chiều cross
    + flex-start: trên cùng chiều cross


flex item:
- flex-grow: làm tăng kich thước item theo trục main bắt đầu từ kich thước flex basis
- flex-shrink: chỉ khả dụng khi các flex tràn ra khỏi container, khi set giá trị cho flex shrink thì các khoảng k của container sẽ k tràn ra ngoài nữa
- flex-basis: đưuọc dùng đẻ xác định kích thước của 1 item trước khi  flex-grow và flex-shrink được áp dụng, mặc định là auto, nếu dã set giá trị heigh, width thì flex-basis sẽ đc gán gía trị đó

- flex: là viết tắt của 3 cái trên 1 1 auto (grow shrink basis)

- order: thay đổi thứ tự các flex element


** CSS Position có 5 giá trị chính
- static: tuân theo normal flow của trang, thay đổi các thuộc tính top, left, right, bottom, z-index không làm thay đổi thuộc tính element đó.
- relative: có thể thay đổi các thuộc tính top, left, right, bottom, z-index so với ban đầu
- absolute: loại bỏ khỏi dòng chảy thông thường của trang, và k gian dưới sẽ bị đẩy lên chỗ set position là absolute, vị trí hiển thị của element sẽ tương đôi vs thẻ cha có các thuộc tính trong (relative, absolute, fixed, sticky)
- fixed: loại bỏ khỏi dòng chảy của trang và hiển thị tương đối vs root element
- sticky: cuộn trang giữa nguyên nhưng chỉ đứng ở khu vực container


*** Sass là 1 tiền xử lý css  nó cung cấp cho chúng ta rất nhiều: khả năng viết code lồng nhau, tạo biến, khả năng chia tách file thành các module nhỏ hơn, và ...