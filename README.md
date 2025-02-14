# Digital-Legal-Inclusion-Transforming-Access-in-Underserved-Areas
Using technology to ensure legal information and services are available to all, bridging the digital divide.
from fastapi import FastAPI
//pythoncode
app = FastAPI()

@app.get("/")
def read_root():
    return {"message": "Welcome to our Legal Access API!"}

@app.get("/legal-info/{item_id}")
def read_item(item_id: int):
    return {"item_id": item_id, "info": f"Details about legal topic {item_id}"}

if __name__ == "__main__":
    import uvicorn
    uvicorn.run(app, host="0.0.0.0", port=8000)


    //javascript
  <!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Simple JavaScript Example</title>
</head>
<body>
    <h1>Welcome to Our Legal Access Platform</h1>
    <button onclick="showAlert()">Click Me!</button>

    <script>
        function showAlert() {
            alert("Button clicked! Welcome to our platform!");
        }
    </script>
</body>
</html>
