# Extended Intelligences II: AI & LLM's - Reflection

The default setting in my mind for anything Artificial Intelligence related was set to negative. From all the harsh realities about the physical infrastructure and the massive energy consumption it's built on, I perceived it as an existential threat to our human connection with nature. Even though I use it on a daily basis for the most trivial curiosities, the same way I used Google search in the past, I still instinctively registered it as a big bad energy. I've also gotten sick of it constantly being discussed around in numerous classes, without truly understanding the architecture of it all. The technicalities of what an LLM really is felt out of reach, until this particular course – it demystified the concept for me and truly changed my understanding of the construct of an LLM. It helped me properly understand what really goes into one and the multitude of ways it can be used.

The theory of it all is quite interesting and I think the way it was presented made it easy and interesting to follow. Concepts of setting up LLM personas, multi-agentic architecture and the employment of multiple persona panels to safeguard the outputs of LLM's were all brand new to me, and they helped me understand how an LLM's frame of reference is constructed. It also somehow gave me a glimmer of hope, despite the fact that it currently may not be exercised, that these systems can somehow be built to be more ethical and intentional. The conversations and debates that arose from discussing our thoughts on the persona panel building were very eye-opening and critical for us to acknowledge the responsibility but also the effectivity of these persona panels. A big thank you to Chris & Pietro for structuring and presenting this class in an engaging and interesting manner, especially the theoretical aspect.

## Group Project

Part of the course was the group project. It was enjoyable to experiment with some of these concepts hands on and understand what it means to work with agent builders.

The concept of my group's project was to create a "Weather Radio" – a tool that combines information from a localized light resistance sensor, the current geolocation and research surrounding mood supporting music to curate music suggestions. The intention was for the playlist to function as a mood stabilizer, helping to regulate your mood based on the local weather conditions and helping set up for a positive day. Initially stemming from the idea of monitoring daily sunlight levels and getting some kind of sound as a corresponding output, the idea eventually evolved into gathering hyper-local sunlight data levels and the general weather forecast of the current city to propose a corresponding playlist to help optimize your mood for the day. Due to time constraints, we had to scale it down to a song from an entire playlist, but that is definitely an area for expansion in the future and I would say we learnt a lot regardless.

One thing I really appreciated was the push to work with the Raspberry Pico, because that is definitely something we were not familiar with and might have been a little intimidated to work with in the beginning. Usually, I shy away from working with electronics and coding because I know it is not my strong suit, but this time I decided to challenge myself and break that barrier. Once we started working with it, we realized it wasn't hard at all and both Pietro & Chris were very helpful and supportive throughout the entire process.

Beste & I worked on connecting the Raspberry Pico, getting the LDR sensor to give analog outputs of the sunlight levels and getting that information on to a server online. We found the code and the schematic diagram of how to connect the LDR sensor to the raspberry pico in the following link: [https://docs.sunfounder.com/projects/pico-2w-kit/en/latest/pyproject/py_photoresistor.html](https://docs.sunfounder.com/projects/pico-2w-kit/en/latest/pyproject/py_photoresistor.html). The information hosted on the online IP address was then used in a three-agent system built on Open AI's Agent Builder, which is broken down in the diagram below.

While I wish we had more time to work on the project, it was the start of something great nevertheless and it is something I would personally love to push forward and develop properly. Personally, I am heavily impacted by sunlight and I find myself chasing light, so a tool like this is something I would greatly appreciate having in my daily routine, as I am sure everyone would. For potential future development, we discussed ideas of the mobility of the LDR sensor to get hyper local data, making it into an artifact that people can take into their day, integrating motivational speech as fuzzy data, integrating it into public transport like buses and allowing the agents to access Barcelona's public database through the internet to create more localized data. I think the project has a lot of potential for expansion and improvement and it would be rewarding to fully bring it to life.

Ultimately, my main take away from all the learnings and discussions of this course is this: artificial intelligence does not have to be the big bad wolf. It really all comes down to one main factor - how we choose to use it. If we approach it ethically and mindfully, it can be a tool for good. Still the real question remains, in our current day and age, are we truly capable of holding ourselves accountable to these ethical standards we preach?

## Code

````python
import machine
import utime

# Initialize ADC on GP28
photoresistor = machine.ADC(28)

while True:
    # Read the analog value (0-65535)
    light_value = photoresistor.read_u16()
    print("Light value:", light_value)
    utime.sleep(0.5)
`````