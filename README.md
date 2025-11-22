# Stock forecasting JS

LSTM Model for stock forecasting and buying simulation inside Tensorflow JS, so everyone can try!

## Stack

Graphic library: [Echarts](https://ecomfe.github.io/echarts-examples/public/index.html), [D3](https://d3js.org/)

CSV parsing: [Papaparse JS](https://www.papaparse.com/)

Linear algebra: [numeric JS](https://github.com/sloisel/numeric), [numJS](https://github.com/cliffordwolf/NumJS), [Tensorflow JS](https://js.tensorflow.org/)

## How-to

1. Clone this folder and just open [index.html](index.html),

Or, go to [huseinhouse.com/stock-forecasting-js](https://huseinhouse.com/stock-forecasting-js/)!

![alt text](screenshot/1.png)

2. Check hyper parameters you want to tune,

![alt text](screenshot/2.png)

3. You can upload any stock CSV, downloaded from Yahoo finance or any website. Any error, please open an issue.

4. Train the model and wait it's fitting!

5. After done training, it will predict where to buy and sell,

![alt text](screenshot/3.png)

Comparing histogram and loss graph,

![alt text](screenshot/4.png)
## Markdown
# Dự Đoán Giá Tiền Mã Hóa Bằng Stacking Ensemble & Multi-Agent System
### Đồ án data

## Tổng quan dự án
Xây dựng hệ thống dự đoán giá Bitcoin & các đồng tiền mã hóa lớn bằng cách kết hợp:
- Deep Learning (LSTM, GRU, Transformer)
- Stacking Ensemble (kết hợp nhiều mô hình)
- Multi-Agent Simulation (mô phỏng hành vi thị trường)
- Realtime Agent (cập nhật & dự báo liên tục)
- Phiên bản chạy trực tiếp trên trình duyệt bằng TensorFlow.js (không cần cài đặt gì)

## Cấu trúc thư mục 
├── agent/              → Các agent cơ bản
├── dataset/            → Dữ liệu giá lịch sử (BTC, ETH, BNB…)
├── deep-learning/      → Mô hình LSTM/GRU/Transformer
├── free-agent/         → Agent tự do
├── misc/               → File hỗ trợ
├── output/ & output-agent/ → Kết quả dự đoán & log
├── realtime-agent/     → Dự đoán realtime (cập nhật mỗi 1–5 phút)
├── simulation/         → Mô phỏng thị trường bằng multi-agent
├── stacking/           → Stacking ensemble (best performer)
└── stock-forecasting-js/ → Demo chạy trực tiếp trên web (TensorFlow.js)

## Demo online 
https://Trananvku2004.github.io/Data-crypto/stock-forecasting-js/  
→ Upload file CSV → Tune hyper-parameter → Train → Xem điểm mua/bán ngay trên biểu đồ!

## Cách chạy local
```bash
# Phần Python
pip install -r requirements.txt
jupyter notebook
# → mở các file .ipynb trong deep-learning/, stacking/, realtime-agent/...

# Phần web (TensorFlow.js)
Chỉ cần mở file stock-forecasting-js/index.html bằng trình duyệt
