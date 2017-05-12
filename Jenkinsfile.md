

```python
pipeline {
    agent { docker 'python:3.5.1' }
    stages {
        stage('build') {
            steps {
                sh 'python --version'
            }
        }
    }
}
```


      File "<ipython-input-1-80b944ddd494>", line 1
        pipeline {
                 ^
    SyntaxError: invalid syntax
    

