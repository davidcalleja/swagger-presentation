##  Y así es como se vería

<section>
    <pre><code yaml hljs>
swagger: '2.0'
info:
  version: 1.0.0
  title: Echo
  description: |
    #### Echos back every URL, method, parameter and header
    Feel free to make a path or an operation and use **Try Operation** to test it. The echo server will
    render back everything.
schemes:
  - http
host: mazimi-prod.apigee.net
basePath: /echo
paths:
  /:
    get:
      responses:
        200:
          description: Echo GET
    post:
      responses:
        200:
          description: Echo POST
      parameters:
        - name: name
          in: formData
          description: name
          type: string
        - name: year
          in: formData
          description: year
          type: string
  /test-path/{id}:
    parameters:
      - name: id
        in: path
        description: ID
        type: string
        required: true
    get:
      responses:
        200:
          description: Echo test-path
    </code></pre>
</section>