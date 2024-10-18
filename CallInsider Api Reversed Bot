import requests
def numberAndComments(countryCode , number):
        headers = {
                'Authorization': 'Basic Y2FsbGlzaW5kZXI6',
                'api-key': '30f75fc0-5ea7-4647-84bb-c4f515cd43cc',
                'Content-Type': 'application/json; charset=UTF-8',
                'Content-Length': '37',
                'Accept-Encoding': 'gzip',
                'User-Agent': 'okhttp/4.10.0'
            }
        data = {
                "i": countryCode,
                "ll": "en",
                "n": number
            }
        response = requests.post("https://api.callinsider.com/api/android/numberAndComments" , headers=headers , json=data)
        return response.json()
def commentGet(countryCode , number):
        headers = {
                'Authorization': 'Basic Y2FsbGlzaW5kZXI6',
                'api-key': '30f75fc0-5ea7-4647-84bb-c4f515cd43cc',
                'Content-Type': 'application/json; charset=UTF-8',
                'Content-Length': '37',
                'Accept-Encoding': 'gzip',
                'User-Agent': 'okhttp/4.10.0'
            }
        data = {
                "i": countryCode,
                "n": number
            }
        response = requests.post("https://api.callinsider.com/api/android/comment/get" , headers=headers , json=data)
        return response.json()

print(numberAndComments("MA" , "0680597173"))
print(commentGet("MA" , "0680597173"))
