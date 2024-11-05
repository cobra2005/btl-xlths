1. Hàm changeChartTimeframe()
Chức năng: Gửi yêu cầu đổi khung thời gian cho biểu đồ (candlestick hoặc line chart).
Cách thức hoạt động: Gửi yêu cầu đến server với khung thời gian mong muốn.
Trong đó:

/api/change-timeframe là URL API để yêu cầu thay đổi khung thời gian.
timeframe là thông số truyền vào (ví dụ: 1m, 5m, 1d, v.v.).
updateChartWithNewTimeframe() là hàm giả định để cập nhật dữ liệu biểu đồ sau khi đổi khung thời gian (có thể tùy chỉnh theo cấu trúc thực tế của bạn).

2. Hàm fetchChartData()
Chức năng: Gọi API để lấy dữ liệu cho biểu đồ hiện tại.
Cách thức hoạt động: Gửi yêu cầu đến server để lấy dữ liệu biểu đồ dựa trên khung thời gian hiện tại.
Trong đó:

/api/get-chart-data là URL API để lấy dữ liệu biểu đồ.
updateChartWithData() là hàm giả định để cập nhật biểu đồ với dữ liệu mới (thực tế bạn có thể gọi chart.updateSeries() của ApexCharts với dữ liệu này).

3. Hàm fetchLineChartData()
Chức năng: Gửi yêu cầu lấy dữ liệu cho biểu đồ dạng line.
Cách thức hoạt động: Tương tự như fetchChartData(), nhưng dành riêng cho dữ liệu biểu đồ line.

Trong đó:

/api/get-line-chart-data là URL API để lấy dữ liệu biểu đồ line.

updateLineChartWithData() là hàm giả định để cập nhật dữ liệu biểu đồ line.
