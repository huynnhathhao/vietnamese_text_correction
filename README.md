# vietnamese_text_correction
Hard-masked XLM-R for Vietnamese Text Correction

## Chạy mô hình với model được huấn luyện sẵn
1. Tải các file trong thư mục sau về : https://drive.google.com/drive/folders/1pFecTPiMqcg7sIeebkM8QSerRN1pfTlb?usp=sharing
2. Tải về file notebook HardMasked_predict.ipynb, đặt chung thư mục với thư mục vừa tải về, Khuyến khích chạy trên Google Colab!

## Chi tiết các files
`Sua loi chinh ta tu dong.pdf` và `Spelling Error Correction using XLM-RoBERTa.pdf` trình bày chi tiết thí nghiệm và kết quả.

`crawltext.ipynb` chứa code thu thập dữ liệu từ các trang báo điện tử

`CreateData.ipynb` chứa code dùng để tạo dữ liệu training.

`Training_detector.ipynb` chứa code để huấn luyện detector.

`HardMasked_predict.ipynb` dùng để predict, sau khi đã huấn luyện detector.

`Spelling Error Correction using XLM-RoBERTa.pdf` report phương pháp.

Link bài viết tutorial: https://huynhnhathao.github.io/myblogs/2021/01/20/vietnamese-spelling-error-correction.html

## Train tokenizer và mô hình từ đầu

### Train spm tokenizer

Tải về file text: https://drive.google.com/file/d/1mCkOhA8gYo01sdCuDmGyhCWw1aiDtF7Q/view?usp=sharing, dùng notebook CreateData.ipynb để huấn luyện spm tokenzer.

### Train detector

Để huấn luyện lại detector, cần tạo dữ liệu các từ sai chính tả theo hướng dẫn như trong file CreateData.ipynb.
