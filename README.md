from flask import Flask, render_template

app = Flask(__name__)

@app.route('/')
def home():
    return "<h1>Chào mừng bạn đến với web thử nghiệm!</h1>"

@app.route('/about')
def about():
    return "<p>Đây là trang giới thiệu. Bạn có thể chỉnh sửa nội dung này!</p>"

if __name__ == '__main__':
    app.run(debug=True)
