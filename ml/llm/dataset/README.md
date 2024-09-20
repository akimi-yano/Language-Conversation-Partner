# Dataset

For the memory retrieval mechanism, I created a method to automatically store data from past conversations in `memory.json`, and, using this data, generate the user's memory index `{user_name}_index`. The technologies utilized are LLamaIndex and the text-embedding-ada model.

The data for the memory retrieval mechanism is designed to grow automatically as the user interacts more with the robot, starting with no data for new users.

Here is the schema and an example of the data stored in `memory.json`:

```json
{
  "mimi": {
    "name": "mimi",
    "history": {
      "2024-09-19": [
        {
          "query": "I love coding challenges",
          "response": "That's great to hear! Coding challenges can be a fun and engaging way to sharpen your programming skills. Is there a specific type of coding challenge you enjoy the most?"
        }
      ]
    },
    "summary": {
      "2024-09-19": {
        "content": "mimi enjoys coding challenges as a way to sharpen programming skills."
      }
    },
    "personality": {
      "2024-09-19": "Based on the dialogue, Mimi appears to be enthusiastic and passionate about coding challenges, indicating traits of curiosity and a love for problem-solving. She seems motivated and driven to improve her programming skills. \n\nIn response to Mimi's enthusiasm, the AI Companion acknowledges her passion for coding challenges and encourages her by validating her interest and offering further engagement by asking about her favorite type of coding challenge. This response strategy aims to maintain Mimi's enthusiasm and motivation by showing genuine interest in her interests and providing opportunities for her to share more about her preferences.\n\nOverall, it is important to continue supporting Mimi's passion for coding challenges by providing encouragement, validation, and opportunities for further exploration in order to foster her growth and development in programming."
    },
    "overall_history": "Mimi enjoys coding challenges to improve programming skills.",
    "overall_personality": "User Personality: Enthusiastic, passionate about coding challenges, curious, loves problem-solving, motivated, driven to improve programming skills.\n\nResponse Strategy: Acknowledge passion, validate interest, ask about favorite coding challenges, offer further engagement to maintain enthusiasm and motivation."
  }
}
```