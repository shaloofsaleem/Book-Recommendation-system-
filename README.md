## 
Book-Recommendation-system
<br>
<p align='center'>
<img src="https://github.com/Jauharmuhammed/README-Template/blob/main/assets/Mockup-website.png" width='70%' >
</p>
<br>

A book recommendation system is a type of recommender system that suggests books to users based on their preferences and past behavior. The goal of a book recommendation system is to help users discover new books that they might be interested in reading.



- Lorem ipsum dolor sit amet, consectetur adipiscing elit.
- In sit amet cursus ex.
- Maecenas id lacus ut diam placerat lobortis ac quis nisl.
-  Nam tristique vulputate ante at malesuada.
- imperdiet elit posuere ut.

<br>

### Built With

![Python](https://img.shields.io/badge/Python%20-%2314354C.svg?style=for-the-badge&logo=python&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![HTML5](https://img.shields.io/badge/HTML5%20-%23E34F26.svg?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS%20-%231572B6.svg?style=for-the-badge&logo=css3&logoColor=white)

![Bootstrap](https://img.shields.io/badge/Bootstrap-563D7C?style=for-the-badge&logo=bootstrap&logoColor=white)

  
![Firebase](https://img.shields.io/badge/firebase-%23039BE5.svg?style=for-the-badge&logo=firebase)

![Github Pages](https://img.shields.io/badge/GitHub%20Pages-%23327FC7.svg?style=for-the-badge&logo=github&logoColor=white)
![Git](https://img.shields.io/badge/git-%23F05033.svg?style=for-the-badge&logo=git&logoColor=white)
![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)
![Canva](https://img.shields.io/badge/Canva-%2300C4CC.svg?style=for-the-badge&logo=Canva&logoColor=white)
![Visual Studio Code](https://img.shields.io/badge/Visual%20Studio%20Code-0078d7.svg?style=for-the-badge&logo=visual-studio-code&logoColor=white)



<br>

## Running this project

Book-Recommendation-system Project.
To build a book recommendation system, you need a large dataset of books, their authors, genres, descriptions, ratings, and any other relevant information. You also need to preprocess the data to clean it and convert categorical variables to numerical ones. Then you choose an appropriate algorithm, such as content-based filtering or collaborative filtering, and train your model on the preprocessed dataset.

## Collect Data/ Import Library: 
Collect a dataset of books, their authors, genres, descriptions, ratings, and any other relevant information that will help you build a recommendation system.



```
import numpy as np
import pandas as pd
```

### Preprocess Data:
Clean the data and preprocess it for use in your recommendation system. This may include tasks such as removing duplicates, filling in missing values, and converting categorical variables to numerical ones.
```
Popularity Based Recommender System
Collaborative Filtering Based Recommender System
```

### Choose a Recommendation Algorithm
 There are many recommendation algorithms to choose from, such as content-based filtering, collaborative filtering, and matrix factorization. Choose the one that best fits your needs.

```
from sklearn.metrics.pairwise import cosine_similarity
```

### Train Your Model And save in files:
Train your recommendation system on your preprocessed dataset using the chosen algorithm.
```
import pickle
pickle.dump(pt,open('pt.pkl','wb'))
pickle.dump(book,open('books.pkl','wb'))
pickle.dump(similarity_scores,open('similarity.pkl','wb'))
```

Then install the project dependencies with

```
pip install -r requirements.txt
```

### Load the trained model:
Load the trained machine learning model into your Flask application. You can use a library like pickle to serialize your model and save it to disk, then load it into your Flask application when it starts up.
```
import pickle
from flask import Flask, request, render_template

# Load the trained model from disk
with open('model.pkl', 'rb') as f:
    model = pickle.load(f)

# Create a new Flask application
app = Flask(__name__)

# Define a route for book recommendations
@app.route('/recommend')
def recommend_books():
    # Get user input from the request arguments
    title = request.args.get('title')
    author = request.args.get('author')
    
    # Use the model to generate recommendations
    recommendations = model.predict(title, author)
    
    # Render the recommendations as HTML output
    return render_template('recommendations.html', recommendations=recommendations)

# Run the Flask application
if __name__ == '__main__':
    app.run(debug=True)

```
Create a user with manage.py
```
python manage.py createsuperuser
```

To build a book recommendation system, you need a large dataset of books, their authors, genres, descriptions, ratings, and any other relevant information. You also need to preprocess the data to clean it and convert categorical variables to numerical ones. Then you choose an appropriate algorithm, such as content-based filtering or collaborative filtering, and train your model on the preprocessed dataset.

Once your model is trained, you can build a user interface that allows users to input their preferences and see book recommendations based on those preferences. This user interface can be built using a web framework like Flask, and can be deployed on a cloud service like Heroku.

Overall, a book recommendation system can be a powerful tool for helping users discover new books and improving their reading experience.




<br>

## Screenshots



<table width="100%"> 
<tr>

<td width="50%">
<p align="center">
Light Mode
</p>
<img src="https://github.com/Jauharmuhammed/README-Template/blob/main/assets/light%20Mode.png">  
</td>
  <td width="50%">      
<p align="center">
Dark Mode
</p>
<img src="https://github.com/Jauharmuhammed/README-Template/blob/main/assets/dark-mode.png">
</td> 
</table>
<br/>

## Contact

<div align='left'>

<a href="https://linkedin.com/in/jauharmuhammed" target="_blank">
<img src="https://img.shields.io/badge/linkedin-%2300acee.svg?color=405DE6&style=for-the-badge&logo=linkedin&logoColor=white" alt=linkedin style="margin-bottom: 5px;"/>
</a>
	
<a href="https://twitter.com/jauharmuhammed_" target="_blank">
<img src="https://img.shields.io/badge/twitter-%2300acee.svg?color=1DA1F2&style=for-the-badge&logo=twitter&logoColor=white" alt=twitter style="margin-bottom: 5px;"/>
</a>
	
<a href="mailto:jauharmuhammedk@gmail.com" target="_blank">
<img src="https://img.shields.io/badge/gmail-%23EA4335.svg?style=for-the-badge&logo=gmail&logoColor=white" t=mail style="margin-bottom: 5px;" />
</a>
	
		
<a href="https://codepen.io/jauharmuhammed" target="_blank">
<img src="https://img.shields.io/badge/codepen-%23000000.svg?style=for-the-badge&logo=codepen&logoColor=white" t=mail style="margin-bottom: 5px;" />
</a>

</div>
