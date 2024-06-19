# Anime-All-Stars-Turbo-Track-Showdown

### Anime Cutting up Game - Racing Game: 
* All anime -  intertextuality
* Anime type cars
* Game Name - Anime All-Stars: Turbo Track Showdown
  
### Description: 
* It's a 2D game where different anime characters have their cars.
* You can pick which car you want to use
* You will race a different Car
* There will be obstacles (other cars on a highway).

## Key Features:
### Diverse Character Roster:
* Gojo Satoru (Jujutsu Kaisen), Naruto Uzumaki (Naruto), Ichigo Kurosaki (Bleach), Luffy (One Piece), and many more.
* Each character has unique abilities that can be used during races to gain an advantage.

### Customizable Vehicles:
* Characters come with signature vehicles that can be customized and upgraded.
* Unlock particular parts and skins by completing races.

### Motivation: 
* Karl and I both love anime
* We both love racing games
* I can make designs, which I'm very passionate about. (Cristian)
* We both loved coding games. 
*nterest in anything car-related.

### Game Concept:
"Anime All-Stars: Turbo Track Showdown" is an exhilarating racing game that combines iconic characters from various anime universes. Players can select from a roster of beloved anime heroes and villains, each with unique abilities and custom vehicles, to compete in high-speed races across fantastical tracks inspired by their respective worlds.

### Sketches/Designs: 
![AnimeRacingGameCopy1](https://github.com/cristia-alvarado/Anime-All-Stars-Turbo-Track-Showdown/assets/167561717/807e0ff6-9130-4fee-8a9e-75909cda1181) 
![AnimeControlScreen (1)](https://github.com/cristia-alvarado/Anime-All-Stars-Turbo-Track-Showdown/assets/167561717/cdee8d9b-9658-4f3b-b805-76bafac2e276)
![DefeatScreenAnime](https://github.com/cristia-alvarado/Anime-All-Stars-Turbo-Track-Showdown/assets/167561717/e6679c88-538a-466c-b39d-658c17ca7135)
![VictoryAnime](https://github.com/cristia-alvarado/Anime-All-Stars-Turbo-Track-Showdown/assets/167561717/296fe85b-d649-4313-9bcd-5139df72ca87)
![IMG_5881](https://github.com/cristia-alvarado/Anime-All-Stars-Turbo-Track-Showdown/assets/167561717/1490f046-28ff-4425-9e87-79a65a0d6bf1)
![IMG_5891](https://github.com/cristia-alvarado/Anime-All-Stars-Turbo-Track-Showdown/assets/167561717/186b4e1a-2a4a-46b0-ac6e-5a6bd27063c1)
![IMG_5895](https://github.com/cristia-alvarado/Anime-All-Stars-Turbo-Track-Showdown/assets/167561717/2ffdb69d-fc53-4b48-94af-c1e72375e082)
![IMG_6001](https://github.com/cristia-alvarado/Anime-All-Stars-Turbo-Track-Showdown/assets/167561717/3004b627-ec2e-43ba-a3ec-69639c703710)
![GokuCar](https://github.com/cristia-alvarado/Anime-All-Stars-Turbo-Track-Showdown/assets/167561717/126b6b1b-7c2c-4d8f-a7a1-2a94e59daf65)
![EsdeathCar](https://github.com/cristia-alvarado/Anime-All-Stars-Turbo-Track-Showdown/assets/167561717/a53489a9-10e2-43d3-a066-670449a70b5c)
![GojoCar](https://github.com/cristia-alvarado/Anime-All-Stars-Turbo-Track-Showdown/assets/167561717/87fd56d2-101c-4476-a57d-af1d50cab6a6)




### Week 1: 
* Start a Database to organize everything.
* Start the Code.
* This week, I'll start designing the game's screens. (Cristian) 
* Sketch Design Ideas.
* This week we will put the screens into the code.

### Week 2:
* Continue working on the code.
* This week we will work on the actual game part.
* Keep up with the database.
* Continuing Designs.

### Week 3:
* Finish the code.
* Finish up all the rough edges.
* Redesign when needed.


### **Code:**
|     [Open Processing Code](https://openprocessing.org/sketch/2295029) | 

## Database:
### Schema SQL: 
-- Drop the table if it exists
DROP TABLE IF EXISTS "myTable";

-- Create the table
CREATE TABLE "myTable" (
  "place" SERIAL PRIMARY KEY,

  "name" VARCHAR(255) DEFAULT NULL,
  "anime" VARCHAR(100) DEFAULT NULL,
  "car" VARCHAR(255) DEFAULT NULL

);

-- Insert data into the table
INSERT INTO "myTable" ("place", "name", "anime", "car")
VALUES
('1', 'Naruto Uzumaki', 'Naruto', 'Acura NSX'),
  ('2', 'Sung JinWoo', 'Solo Leveling', 'Ultimate Nissan Silvia S15'),
  ('3', 'Son Goku', 'Dragon Ball', '1976 VW Beetle Convertible'),
  ('4', 'Asta Staria', 'Black Clover', 'Bugatti Chiron Crimson'),
  ('5', 'Ichigo Kurosaki', 'Bleach', 'Nissan 180SX'),
  ('7', 'Esdeath', 'Akame GaKill', 'BMW m5'),
    ('8', 'Gojo', 'Jujutsu Kaisen', 'Mercedes-AMG GT Track Car'),
 ('6', 'Frieren The Elf', 'Frieren: Beyond Journeys End', 'White Ferrari Enzo');
 
 
 -- Create the table
CREATE TABLE "iTable" (
  "power" VARCHAR(255) DEFAULT NULL,

  "anime" VARCHAR(255) DEFAULT NULL


);

-- Insert data into the table
INSERT INTO "iTable" ("power", "anime")
VALUES
 ('Rasengan', 'Naruto'), 
  ('Kamekameha', 'Dragon Ball'),
 ('Bankai', 'Bleach'),
(' Anti-Magic', 'Black Clover'),
(' A Torrent Of Unceasing Flame', 'Frieren: Beyond Journeys End'),
('Limitless Void', 'Jujustu Kaisen'),
 ('Shadow Monarch', 'Solo Leveling');

### Query:
SELECT * FROM "myTable"
ORDER BY place ASC;

SELECT * FROM "iTable"

### Link For Database:
[SQL Database](https://www.db-fiddle.com/) 

## Pseudocode

Initialize game setup:

    Create canvas with width and height
    
    Load images and sprites
    
    Load sounds
    
    Setup track elements
    
    Setup player and objects

Main game loop:
    
    Clear the screen
    
    Draw the background
    
    Draw the track
    
    Draw the player car
    
    Draw objects
    
    Handle player movement:
    
        If LEFT arrow key is pressed, turn player car left
        
        If RIGHT arrow key is pressed, turn player car right
   
    Update game elements:
   
        Update player car position
      
        Update object positions
        
        Update track elements
  
    Check collisions:
   
        If player car collides with object or track boundary, handle collision
  
    Update game state:
    
        If player finishes the race, display win sequence
     
        If player loses, display lose sequence


Handle player input:

    If key pressed:
   
        Process key press

Process key press:
   
    If LEFT arrow key is pressed, turn player car left
  
    If RIGHT arrow key is pressed, turn player car right

Trigger win sequence:
 
    Display win message
 
    Play win sound

Trigger lose sequence:
 
    Display lose message
  
    Play lose sound

Utility functions:
  
    Load images and sprites
    
    Load sounds
    
    Setup track elements
    
    Setup player and object
    
    Update player car position
    
    Update object positions
    
    Update track elements
    
    Check collisions
    
    Handle collision






















