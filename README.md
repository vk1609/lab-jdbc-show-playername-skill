![Image description](https://i1.faceprep.in/ProGrad/face-logo-resized.png)

# ProGrad Lab | ProGrad Premier League


## Progression 1:

Create a class called as `Main` with main method 
Create a class called as `skill` with below attributes, 
```
skillld - Long 
skillName - String 
```


## Progression 2:

Include getter and setter method for all the attributes Include constructor with below arguments, public Skill(skillId, skillName) 


## Progression 3:

Create a dao-class called as `SkillDAO` withe below method, 
`public Skill getSkillBylD(Long id)` - Method used to fetch the skill information from the database based on the skill id. 


## Progression 4:

Create a class called as `Player` with below attributes, 
```
playerld - Long 
name - String 
country - String 
skill - Skill 
```
Include getter and setter method for all the attributes Include constructor with below arguments, 
`public Player(Long playerld,String name, String country,Skill skill)` 


## Progression 5:

Create a class called as `PlayerDAO` with below methods, 
`public List<Player> getAllPlayers()` - Method used to fetch all the players and their corresponding skill from the database.


![1 2](https://user-images.githubusercontent.com/61002120/76416050-5807d380-63c0-11ea-8d52-9e8750e800f9.png)


### Note:

Use the below code to retreive the connection details from mysql.properties to establish connection
```
public static Properties loadPropertiesFile() throws Exception {
	Properties prop = new Properties();	
	InputStream in = ConnectionManager.class.getClassLoader().getResourceAsStream("jdbc.properties");
	prop.load(in);
	in.close(); 
	return prop;
}
```    
**Sample Output**
```
 List of all player and their skill
 Id 	Name 		Country 	Skill 
 26 	Aaron Finch 	Australia 	Batting 
 80 	AB de Villiers 	South Africa 	Batting 
 82 	Abu Nechim 	India 		Bowling 
 85 	Adam Milne 	New Zealand 	Bowling 
 16 	Akshdeep Nath 	India 		All Rounder
```
