# DockerFlaskPython-Example
Example code for docker flask python setup.

## Tutorials
This sample code was created using the following tutorials.
1. https://code.visualstudio.com/docs/python/tutorial-flask
1. https://code.visualstudio.com/docs/containers/quickstart-python

## Testing locally
Setup the Python:Flask launch json and test using intellij debugger.

```
{
    // Use IntelliSense to learn about possible attributes.
    // Hover to view descriptions of existing attributes.
    // For more information, visit: https://go.microsoft.com/fwlink/?linkid=830387
    "version": "0.2.0",
    "configurations": [
        {
            "name": "Python: Flask",
            "type": "python",
            "request": "launch",
            "module": "flask",
            "env": {
                "FLASK_APP": "hello_app.webapp",
                "FLASK_ENV": "development",
                "FLASK_DEBUG": "0"
            },
            "args": [
                "run",
                "--no-debugger"
            ],
            "jinja": true
        }
    ]
}
```

## Run Docker
docker run -d -p 5000:5000 helloflask