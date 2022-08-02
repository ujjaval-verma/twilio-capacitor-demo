# Twilio-Capacitor Demo

Demo Twilio based WebRTC video conferencing app with ability to capture snapshots natively

## Running the application

You'll need Python3 to get this running. To install the required
dependencies:

```
python3 -m venv venv  # create a virtual environment
source venv/bin/activate
pip install -r requirements.txt
```

Next, create a `.env` file. You'll put your account
credentials in that file, so that the Flask server can
connect to Twilio.

```
touch .env
```

In the .env file, you'll want these credentials:

```
TWILIO_ACCOUNT_SID=<your account SID>
TWILIO_API_KEY=<your api key>
TWILIO_API_SECRET=<your api key secret>
```

You can find your account SID in the [Twilio Console Dashboard](https://www.twilio.com/console).

You can create a new API key and get the secret through the
[Twilio Console](https://www.twilio.com/console/project/api-keys).

To run the Flask server:

```
source venv/bin/activate
python server.py
```

This will start a server that you can access on your
local machine at port 5000 (`localhost:5000`). You can view the application
at [http://localhost:5000](http://localhost:5000).

This app users Client Side Room Creation. Make sure client side room creation
is enabled in the [Twilio Console](https://www.twilio.com/console/video/configure).


