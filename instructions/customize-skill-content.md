# Build An Alexa Quiz Game Skill
<img src="https://m.media-amazon.com/images/G/01/mobile-apps/dex/alexa/alexa-skills-kit/tutorials/quiz-game/header._TTH_.png" />

Build an engaging skill that quizes a user with facts about any topic. Alexa will quiz the user with these facts at random and test their knowledge.

## Customize the Skill to be Yours

At this point, you should have a working copy of our Quiz Game skill.  In order to make it your own, you will need to customize it with data and responses that you create.  Here are the things you will need to change:

1.  **New sentences to respond to your users.** There are several sentences and responses that you will want to customize for your skill.

    1. Navigate to the **Code** tab again, and expand the project folder on the left to `Skill Code/lambda/alexa`.

    2. Open **[data.py](../lambda/py/alexa/data.py)**

    3. We are going to be focusing on the contents of lines `255-286`, which contain the response strings used by the Skill. In this example, we are going to change the `EXIT_SKILL_MESSAGE`, said when the user is exiting the skill, to "Thanks for playing, come back later to test your knowledge!". This would result in the following change:

    Before:
     ```py
     ...
     ...,
     EXIT_SKILL_MESSAGE = ("Thank you for playing the United States Quiz Game!  "
                         "Let's play again soon!")
     ...,
     ...
     ```

    After:
     ```py
     ...
     ...,
     EXIT_SKILL_MESSAGE = ("Thanks for playing, "                     <-- CHANGED
                         "come back later to test your knowledge!")   <-- CHANGED
     ...,
     ...
     ```

     After you're done editing all of the files necessary, as before, make sure to press **Save**, **Deploy**, and navigate back to the **Testing** tab. When you relaunch the quiz skill and exit, Alexa will say "Thanks for playing, come back later to test your knowledge!" instead of "Thank you for playing the United States Quiz Game! Let's play again soon!". You can edit more than just the `EXIT_SKILL_MESSAGE`, so feel free to customize all of the messages within lines `255-313` to make it your own!

2.  **New language.** If you are creating this skill for another language other than English, you will need to make sure Alexa's responses are also in that language.

    - For example, if you are creating your skill in German, every single response that Alexa makes has to be in German. You can't use English responses or your skill will fail certification.

3. **Once you have customized the skill's data, languages and/or sentences, return to the [Amazon Developer Portal](https://developer.amazon.com/alexa/console/ask?&sc_category=Owned&sc_channel=RD&sc_campaign=Evangelism2018&sc_publisher=github&sc_content=Survey&sc_detail=fact-nodejs-V2_GUI-5&sc_funnel=Convert&sc_country=WW&sc_medium=Owned_RD_Evangelism2018_github_Survey_fact-nodejs-V2_GUI-5_Convert_WW_beginnersdevs&sc_segment=beginnersdevs) and select your skill from the list.**

4.  **Click on "Distribution" in the top navigation to move on to the publishing and certification of your skill.**


[![Next](https://m.media-amazon.com/images/G/01/mobile-apps/dex/alexa/alexa-skills-kit/tutorials/general/buttons/button_next_publication._TTH_.png)](./submit-for-certification.md)

