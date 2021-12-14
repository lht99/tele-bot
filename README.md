## tele-bot

# Hướng dẫn
Chỉ cần deploy vào heroku để sử dụng bot

# Tạo app trên Heroku
1. Tạo app trên Heroku: https://dashboard.heroku.com/new-app
Tiếp theo chúng ta sẽ có link của app có dạng: https://yourheroku.herokuapp.com/

2. Thay **yourheroku** bằng tên app heroku tạo ở bước 1 trong dòng lệnh sau:
updater.start_webhook(listen="0.0.0.0", port=int(PORT), url_path=TOKEN, webhook_url="https://yourheroku.herokuapp.com/" + TOKEN)
_Sau khi hoàn thành việc bổ sung mã TOKEN và đường dẫn webhook thì tiến hành bước 3_

3. Vào app vừa tạo ở trên heroku, ở tab Deploy chọn git sau đó deploy vào heroku để sử dụng nhé.

# Lấy bot TOKEN
Vào botfather của telegram để lấy TOKEN
