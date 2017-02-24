# Info-Wars-Stream-Alexa
Streaming infowars app


{
    "intents": [
        {
            "intent": "AMAZON.PauseIntent"
        },
        {
            "intent": "AMAZON.ResumeIntent"
        }
    ],
  		"version": "1.0",

  "sessionAttributes": {},

  "response": {

    "outputSpeech": {

      "type": "PlainText",

      "text": "Playing info wars."

    },

    "card": {

      "type": "Simple",

      "title": "Play Audio",

      "content": "Playing Info Wars."

    },

    "reprompt": {

      "outputSpeech": {

        "type": "PlainText",

        "text": null

      }

    },

    "directives": [

      {

        "type": "AudioPlayer.Play",

        "playBehavior": "ENQUEUE",

        "audioItem": {

          "stream": {

            "token": "this-is-the-audio-token",

            "url": "http://stream-mp3.infowars.com/listen.pls",

            "offsetInMilliseconds": 0

          }

        }

      }

    ],

    "shouldEndSession": true

  }

}
