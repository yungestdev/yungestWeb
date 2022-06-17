Hi, sorry to tell you that this method to run the server has been deprecated to give the possibility to run other apps in one file to the user:
```python
    app.run("127.0.0.1", 8070, app)
```

Please use this instead

```python
    run_webapp("127.0.0.1", 8070, app)
```