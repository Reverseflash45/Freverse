<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>First Rafi's website</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f4f4f4;
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            overflow-x: hidden; /* Prevent horizontal scrolling */
        }

        header {
            background-color: #0084ff;
            color: white;
            padding: 10px 0;
            text-align: center;
        }
        nav {
            background-color: #333;
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
        }
        nav a {
            color: white;
            padding: 14px 20px;
            text-align: center;
            text-decoration: none;
            flex: 1;
            min-width: 120px;
        }
        nav a:hover {
            background-color: #ddd;
            color: black;
        }
        .container {
            padding: 15px; /* Adjusted padding for better mobile view */
            display: none;
            max-width: 100%; /* Ensure container does not exceed screen width */
            margin: 0 auto; /* Center the container */
        }

        footer {
            background-color: #333;
            color: white;
            text-align: center;
            padding: 10px;
            position: fixed;
            bottom: 0;
            width: 100%;
            margin: 0 auto;
            justify-content: center;
            display: flex;
        }
        .active {
            display: block;
        }
        img {
            max-width: 100%;
            height: auto;
            border-radius: 5px;
        }
        @media (max-width: 600px) {
            nav a {
                padding: 10px;
                font-size: 14px;
            }
            header h1 {
                font-size: 24px;
            }
            footer {
                flex-direction: column;
                align-items: center;
            }
        }
    </style>
</head>
<body>
    <header>
        <h1>Welcome to My First website</h1>
    </header>

<nav>
    <a href="javascript:void(0);" onclick="showPage('home')">Home</a>
    <a href="javascript:void(0);" onclick="showPage('My_Stories')">My Stories</a>
    <a href="javascript:void(0);" onclick="showPage('My_Achievements')">My Achievements</a>
    <a href="javascript:void(0);" onclick="showPage('My_Failures')">My Failures</a>
    <a href="javascript:void(0);" onclick="showPage('My_Hobbies')">My Hobbies</a>
    <a href="javascript:void(0);" onclick="showPage('My_Favorites')">My Fav & Unfav</a>
    <a href="javascript:void(0);" onclick="showPage('Things_I_Hate')">Things I Hate</a>
</nav>

<script>
    function showPage(pageId) {
        const sections = document.querySelectorAll('.container');
        sections.forEach(section => {
            section.classList.remove('active');
        });

        const activeSection = document.getElementById(pageId);
        if (activeSection) {
            activeSection.classList.add('active');
        }
    }

    window.onload = function() {
        showPage('home');
    };
</script>

<div class="container" id="home" style="background-color: #f9f9f9; padding: 20px; border-radius: 8px; box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);">
    <h2 style="color: #333; font-size: 1.5em;">Home</h2> <!-- Adjusted font size for better readability -->

    <p style="font-size: 16px; line-height: 1.5;">Welcome to my first website! This is where I practice my skills and share my personal journey. I hope you enjoy exploring the pages and get to know more about me, my achievements, and the ideas I am passionate about.</p>
    <p style="font-size: 16px; line-height: 1.5;">This website serves multiple purposes, including:</p>
    <ul style="padding-left: 20px;">
        <li>Practicing and improving my coding skills</li>
        <li>Introducing myself to the world</li>
        <li>Sharing my ideas and vision with others</li>
        <li>Showcasing my achievements</li>
    </ul>
    <p style="font-size: 16px; line-height: 1.5;">I hope you enjoy this site and feel inspired by the things I am working on!</p>

    <img src="https://media3.giphy.com/media/v1.Y2lkPTc5MGI3NjExZTBhbTd2dmdrcmJyMHBkMmU0c3h1ZWtzYnA0ZGl4bDh2NWM2MWIwcSZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/26ufaKwBoqwQItgic/giphy.gif">
</div>

<div class="container" id="My_Stories" style="background-color: #f9f9f9; padding: 20px; border-radius: 8px; box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);">
    <h2 style="color: #333; font-size: 1.5em;">My Stories</h2> <!-- Adjusted font size for better readability -->

    <h3><b>Introduce</b></h3>
    <p style="text-indent: 45px;">My name is Rafi Fernandito Setiawan, or known as Rafi. My birthplace is Kediri City, located in East Java, on January 26 2005. Since childhood, I have always had high aspirations. Even though I live in simple conditions, my parents always encourage me to dare to achieve my dreams and work hard to make them come true.</p>
    <h3><b>The period of my life in kindergarden</b></h3>
    <p style="text-indent: 45px;">My childhood was filled with playing in the rice fields and traveling around the village on a bicycle with my friends after school, and reciting the Koran every evening after sunset. However, the desire to learn always burned within me. I have always been a diligent student at school, even though I often only had limited textbooks. I always study every time I come home from studying the Koran, more precisely I always study from 7 to 9, then I sleep. I wake up at 4 am to study, pray, and prepare my needs to go to school.</p>
    <h3><b>The period of my life in elementary school</b></h3>
    <p style="text-indent: 45px;">Not only did I struggle in the academic field, when I was in elementary school, I practiced non-academic fields such as chess, modern dance and scouting activities. For chess competitions I have won 4th place, for modern dance I have qualified up to city level, and for scouting I have represented my school in simultaneous camping events. I also took part in academic competitions and won several competitions, until at the end of the class when junior high school simultaneously held a PPDB independent test, I took part and only one school passed and continued to my favorite school via the PPDB independent test route.</p>
    <h3><b>The period of my life in junior high school</b></h3>
    <p style="text-indent: 45px;">When I was in junior high school, I didn't have much time because class 8, semester 2, was on holiday for 2 years. However, when I was in grade 7, I qualified to represent my school in a mathematics competition at the national level with my friends. Then when I was in grade 8, semester 1, I took drama training and podcast training. But when it was time to perform, the school was closed for 2 weeks, and at that time I trained myself again, but it turned out that those 2 weeks turned into 2 years.</p>
    <p style="text-indent: 45px;">Because there were no independent PPDB selection tests from my favorite high school or national exams due to the pandemic, I relied more on the national charter that I got in grade 7 rather than my report card grades, where the scores were mixed because at that time the pandemic. Luckily, thanks to this charter, I was accepted into my favorite high school in my area via the achievement route.</p>
    <h3><b>The period of my life in Senior high school</b></h3>
    <p style="text-indent: 45px;">When I was in high school I wanted to try something new, namely organizations. I took part in the selection to become a student council administrator and I was accepted. When I took office, I created a joint work program with other members of the student council management and thanks to God's permission, the events we created were all successful. There was 1 event where I was the representative of the committee and 1 event where I was chairman of the committee, both of which were equally busy and tired, but when the event was successfully carried out in sequence, the tiredness disappeared and became a feeling of joy.</p>
    <p style="text-indent: 45px;">After completing high school, I tried hard to get a scholarship to go to college. Thanks to hard work and support from my family, I managed to get a scholarship even though the scholarship was from an individual, not from an institution. There, I chose to study informatics, according to my interests and talents.</p>
    <h3><b>The period of my life in University</b></h3>
    <p style="text-indent: 45px;">When I was in my first semester of college, I took part in the PIMNAS x AEC committee selection and I passed by becoming a member of the PIMNAS x AEC committee in the field of PDD which was tasked with carrying out documentation which was carried out during pre-event until after the event started. Starting while the meeting was taking photos for ID cards, to taking photos of the committee after the event was over.</p>
</div>

<div class="container" id="My_Achievements" style="background-color: #f9f9f9; padding: 20px; border-radius: 8px; box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);">
    <h2 style="color: #333; font-size: 1.5em;">My Achievements</h2> <!-- Adjusted font size for better readability -->

    <ul>
        <h3><b>My achievements during elementary school</b></h3>
        <p>1. Top 10 city level champion of elementary school dance</p>
<div style="border: 2px solid #ccc; border-radius: 8px; padding: 5px; display: inline-block; margin: 10px;">
    <img src="sd1.jpg" alt="image" height="210" width="420" style="border-radius: 5px;"/>
</div>

        <p>2. Become a sponsor of Antangin Junior product</p>
<div style="border: 2px solid #ccc; border-radius: 8px; padding: 5px; display: inline-block; margin: 10px;">
    <img src="sd2.jpg" alt="image" height="210" width="420" style="border-radius: 5px;"/>
</div>

        <p>3. Representatives in inter-school scouting activities</p>
<div style="border: 2px solid #ccc; border-radius: 8px; padding: 5px; display: inline-block; margin: 10px;">
    <img src="sd3.jpg" alt="image" height="210" width="420" style="border-radius: 5px;"/>
</div>

    </ul>
    <ul>
        <h3><b>My achievements during junior high school</b></h3>
        <p>1. Became a semifinalist in the national mathematics competition</p>
<div style="border: 2px solid #ccc; border-radius: 8px; padding: 5px; display: inline-block; margin: 10px;">
    <img src="smp2.jpg" alt="image" height="210" width="420" style="border-radius: 5px;"/>
</div>

        <p>2. Became a finalist in the national mathematics competition</p>
<div style="border: 2px solid #ccc; border-radius: 8px; padding: 5px; display: inline-block; margin: 10px;">
    <img src="smp1.jpg" alt="image" height="210" width="420" style="border-radius: 5px;"/>
</div>

    </ul>
    <ul>
        <h3><b>My achievements during senior high school</b></h3>
        <p>1. Top 7 national mathematics olympiad</p>
<div style="border: 2px solid #ccc; border-radius: 8px; padding: 5px; display: inline-block; margin: 10px;">
    <img src="SMA (3).jpg" alt="image" height="210" width="420" style="border-radius: 5px;"/>
</div>

        <p>2. Top 3 national mathematics olympiad</p>
<div style="border: 2px solid #ccc; border-radius: 8px; padding: 5px; display: inline-block; margin: 10px;">
    <img src="SMA (4).jpg" alt="image" height="210" width="420" style="border-radius: 5px;"/>
</div>

        <p>3. Finisher in the silver category in the running competition</p>
<div style="border: 2px solid #ccc; border-radius: 8px; padding: 5px; display: inline-block; margin: 10px;">
    <img src="SMA (5).jpg" alt="image" height="210" width="420" style="border-radius: 5px;"/>
</div>

        <p>4. Become student council administrator for 1 period</p>
<div style="border: 2px solid #ccc; border-radius: 8px; padding: 5px; display: inline-block; margin: 10px;">
    <img src="SMA (6).jpg" alt="image" height="210" width="420" style="border-radius: 5px;"/>
</div>

        <p>5. Representative in the competition for college subjects majoring in industrial engineering</p>
<div style="border: 2px solid #ccc; border-radius: 8px; padding: 5px; display: inline-block; margin: 10px;">
    <img src="SMA (7).jpg" alt="image" height="210" width="420" style="border-radius: 5px;"/>
</div>

        <p>6. Passed the office test with an A grade</p>
<div style="border: 2px solid #ccc; border-radius: 8px; padding: 5px; display: inline-block; margin: 10px;">
    <img src="kuliah.jpg" alt="image" height="210" width="420" style="border-radius: 5px;"/>
</div>

    </ul>
    <ul>
        <h3><b>My achievements during college</b></h3>
        <p>1. National committee certificate (PIMNAS x AEC)</p>
<div style="border: 2px solid #ccc; border-radius: 8px; padding: 5px; display: inline-block; margin: 10px;">
    <img src="PIMNAS.jpg" alt="image" height="210" width="420" style="border-radius: 5px;"/>
</div>

    </ul>
    <p>These are just a few of the steps I’ve taken to grow as a developer, and I am excited to see what the future holds!</p>
</div>

<div class="container" id="My_Failures" style="background-color: #f9f9f9; padding: 20px; border-radius: 8px; box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);">
    <h2 style="color: #333; font-size: 1.5em;">My Failures</h2> <!-- Adjusted font size for better readability -->

    <p>Here I will mention things that made my life fail in the past.:</p>
    <li><strong>Lack of life planning:</strong></li>
    <p style="text-indent: 45px;">When I was still a teenager, I really underestimated the so-called life plan. I just lived my days normally without a plan and without ambition which caused my life at that time to be very chaotic.</p>
    <li><strong>Taking relationships for granted:</strong></li>
    <p style="text-indent: 45px;">This also happened when I was still a teenager. I used to be a very closed and introverted person, even my friends and family also called me anti-camera because I really didn't want to get involved with other people in real life or social media. This caused me to not know enough people in high school which made it difficult for me to find information about something.</p>
    <li><strong>Not focusing on myself:</strong></li>
    <p style="text-indent: 45px;">When I was still in high school and in 3rd grade, I had someone I liked and I focused on the person I liked by honing the skills that the person I liked liked, which might not be useful in the future.</p>
    <li><strong>Too crazy about hobbies and doesn't hone skills:</strong></li>
    <p style="text-indent: 45px;">This happened when I was still in high school and I really liked running and cycling and this resulted in me always honing those skills and being reluctant to study school material.</p>
    <p></p>
</div>

<div class="container" id="My_Hobbies" style="background-color: #f9f9f9; padding: 20px; border-radius: 8px; box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);">
    <h2 style="color: #333; font-size: 1.5em;">My Hobbies</h2> <!-- Adjusted font size for better readability -->

    <p>The following are some of my hobbies so far:</p>
    <li><strong>Running:</strong></li>
    <p style="text-indent: 45px;">of high school because I wanted to enroll in an official school, but over time this became one of my hobbies. Usually I run when I have a problem or when I'm worried about something. I use running as an outlet for my feelings of unease. During my training, my running was very structured in terms of time, speed and distance. but when I'm in an unstable state of mind I can run anytime and anywhere, besides that my speed and distance in running will also increase if I'm in an unstable state of mind.Why do I say running is my hobby to relieve myself when my mind is confused? That's because since I was in second year of high school I wasn't interested in games or films anymore, I also didn't have a girlfriend or friends who were very, very close so that I could talk about all my problems in high school. My close friends are all suitable for playing, not suitable for telling stories so I vent my chaotic emotions or feelings into running.</p>
    <li><strong>Reading a book:</strong></li>
    <p style="text-indent: 45px;">I have always been a person who is very anti-reading, be it books, comics, novels, and so on. I first started reading books because I was so bored and I didn't get angry or have anything to say. I tried reading it and it turns out it's quite interesting. In the end, reading books became one of my hobbies when I wanted a calm and peaceful atmosphere. I started reading books with business themes, how to think about being a businessman, how to become rich, and so on. Because I really want to do a business that involves coding in the future, I am also little by little interested in the world of business and how to become a businessman. Over time, I became interested in reading books with themes about human life, the experiences of historical figures, and how to change yourself to become a better person.</p>
    <li><strong>GYM:</strong></li>
    <p style="text-indent: 45px;">I started doing workouts in the middle of grade 11, the first time I started doing workouts or going to the gym was to shape my small and weak body into a big and strong body, but over time the reason changed to venting my frustration at something. or something. It's said to be similar to the reason I ran. However, now the reason I have changed is that I shape and train myself to be strong and make myself feel proud of myself in the future because I dared to be consistent in the past. Usually I do this from 3 to 5 in the afternoon at the gym or in my dorm room. The movements I usually do are various variations of push ups, sit ups, skipping, planks, lifting dumbbells, and many other movements that I usually use to build my muscles. Due to my work out habit, I pay attention to every food and drink that enters my stomach. I also started to adjust my sleeping hours, which usually stay up late so that the maximum sleep limit must be under 10 pm.</p>
    <li><strong>Coding:</strong></li>
    <p style="text-indent: 45px;">I have been interested in the world of coding since I was a child. I see people coding and it looks really cool. This is also what caused me to major in informatics engineering when I was in college, I really wanted to be able to code because my interest has been there since I was little. I also want to make this my dream. In the future I want to work in this field with remote work, I am very interested in remote work because there is no need to go out to work, besides that remote work is also very efficient because the market is very wide from various countries. Apart from that, working remotely can also be done anytime and anywhere without thinking about where we are and when we do our work, we just need to pay attention to the latest deadline for the job desk we are taking. If you don't want to delay, we can finish it directly.</p>
</div>

<div class="container" id="My_Favorites" style="background-color: #f9f9f9; padding: 20px; border-radius: 8px; box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);">
    <h2 style="color: #333;">My Favorites and My Unfavorites</h2>
    <p>Some of my favorites and my unfavorite:</p>

    <p style="text-indent: 45px;"></p>
    <strong>Food:</strong>
        <br>favorite: Cheese Burger & Fried Rice
        <br>Unfavorite: Spicy Food

    <p style="text-indent: 45px;"></p>
    <strong>Drink:</strong>
        <br>favorite: Mineral Water
        <br>Unfavorite: Sugary Drink

    <p style="text-indent: 45px;"></p>
    <strong>Taste of Food:</strong>
        <br>favorite: Savory and Salty
        <br>Unfavorite: Spicy

    <p style="text-indent: 45px;"></p>
    <strong>Taste of Drink:</strong>
        <br>favorite: Savory and Salty
        <br>Unfavorite: Sugary
</div>

<div class="container" id="Things_I_Hate" style="background-color: #f9f9f9; padding: 20px; border-radius: 8px; box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);">
    <h2 style="color: #333; font-size: 1.5em;">Things I Hate</h2> <!-- Adjusted font size for better readability -->

    <p>Here are some of the things I dislike and want to express:</p>
    
        <strong>1. A person who breaks a promise</strong>
        <br><p style="text-indent: 45px;">I don't like people who break their promises, especially those who take them too lightly. For example, making an appointment at 7 am but being 45 minutes late. For me, a promise is an undocumented or unwritten contract that must be kept, unless there is an urgent situation that is more important than what was promised.</p>
    
        <strong>2. People who smoke in public</strong>
        <br><p style="text-indent: 45px;">Smoking alone is very detrimental to people around the smoker (passive smokers), let alone smoking in public places, especially while driving. This is very dangerous for pregnant women, young children, people with a history of asthma, the elderly, drivers, and there are many more effects of smoking in public places that are very detrimental to people around the smoker.</p>
</div>

<footer style="background-color: #f4f4f4; color: #333; padding: 20px; text-align: center; position: relative; margin-top: 20px;">

    <p style="margin: 0;">&copy; 2024 Web page Kurosaki Rafi Yeager. All rights reserved.</p>
</footer>


</body>
</html>
