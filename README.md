This is about one possible way to create an ASL dictionary using 3D models.

With an ASL dictionary we'll need to document signs somehow––traditionally, this has been achieved in the past decade with exploration of video documentation and MotionCapture technology (think Hollywood suits with dots all over for 3D models such as shown here, http://www.motionlightlab.com/asl-nursery-rhymes/ | ). My issue with this approach is that while it's wonderful in that it imagines a world of sign language translation and documentation on levels unseen, it's too slow to succeed. We'd need MoCap tech, cameras, people, studio space and more. 

Another issue is that several labs and university groups have spent time and resources into this topic but then they graduate or the lab stutters in time or funding. And because it's not openly available to the communities that are seeking it, progress is delayed another day. I have heard that a big corpus in the works can be located at Boston University. In the UK, the BSL Corpus is government-funded and it exists, today, online, http://www.bslcorpusproject.org/projects/. Words are searchable, so finding english to BSL translations works. But what about all the words without English translations? 

One alternate approach attempted by http://www.motionsavvy.com/ and http://prodeaf.net/ (Brazil) is a database based on gesture recognition technology––this way it's used as a central database for users all over to feed their signs and translations to. The curve seems far faster with this type of idea. The models they use are 3D models as well. However, who decides what happens and which variation of a sign may be best? And new JS libraries that utilize gesture recognition technology like gest.js and movement.js are coming in––making gesture tech more accessible.

So here we are.. I wanted an open source ASL dictionary. Not necessarily a Corpus, where we'd have samples of real work because the time is too much to invest and videos are an inflexible (read: annoying) data format for us to manipulate. Not necessarily an English to ASL dictionary like http://lifeprint.com. 

So clearly we need two things here: 

ASL users and their key input 
3D models 

A way for ASL users to determine the validity of signs is the "5 ASL Parameters". It's technically 4+1 though it seems over time it's become 5. They are: 

location,
handshape,
palm orientation,
movement,
non-manual signals (facial expressions)

so I figure this will be my learning journey. For now, maybe it won't work or make a product but I'm going to wander in the direction of:

A) learning Blender to make 3D hands and models, faces/people later. I do know the industry is heavily inaccessible due to their heavy use of uncaptioned videos, but I believe CGCookie captions their videos. And I could find a book.

B) developing JSON dictionary of signs, using the 5 parameters as key/value pairs. 

  example: 
      {
      "sign": "street",
      "location": "front",
      "handshape": {
        "dominant": "B",
        "passive": "B" },
      "palm-orientation": {
        "left-hand": "right",
        "right-hand": "left"  },
      "movement": "away",
      "facial-expression": ""
    }

This JSON object stores a sign for the word "street". The sign is done in front of you, with both hands flat in a "B" handshape facing each other (sideways, left facing right / right facing left) and moves away from the signer. It's the entry for "street". The idea is that somewhere down the road, this evolves to become a resource where 3D models can be instructed via Unity or some JS => 3D process. 




-------------------------------
the distant future
-------------------------------

For now, do I have an idea what the road will look like from here? I got some, but it's unclear so I'll keep the end goal open. 

The goal is to enable a new wave of technology with ASL interpreting, storytelling and CGI. 
        
        Auto-ASL translations. A chance to open access to the English world––children's stories, 
        
        Virtual ASL interpreters! We have a significant void for small, casual interactions as we cannot have pocket interpreters. Speech to text translation software exist / ASL dictionaries exist, fragmented but still exist––2 + 2 leads one to think basic translation for simple situations isn't too far-fetched a goal. (Also I want my interpreter to be a Blood Elf rogue; it's just a preference.)

        






 


