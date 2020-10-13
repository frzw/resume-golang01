# flask

### 怎么使用的？
- 主要是使用路由的功能。
```

app = Flask(__name__)
 
@app.route('/')
def hello_world():
    return 'Hello World!'
 
if __name__ == '__main__':

```
### 理解
- 轻量级web微框架。