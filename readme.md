# NavGoa Application
## AI Algorithm Powered Application

**NavGoa** is a Full Stack application and a mini prototype of a Google Maps feature. It takes a source and destination and calculates the shortest path while considering various parameters like road conditions and accident zones. The application also estimates the travel time for the selected route. 

We developed a custom algorithm that combines **A*** and **Dijkstra's algorithms**, optimized to reduce time complexity by eliminating unnecessary recursive calls, resulting in a more efficient pathfinding solution.

## Tech Stack

- Django (Backend)
- DRF - Django Rest Framework (API - Application Programming Interface)
- HTML
- CSS
- JS
- JINJA Framework
- SQLite3 (Inbuilt)
- CSS Framework (BootStrap)
- AI Algorithm 
---
## Features

- It uses custom **AI algorithm** to predict the current best shortest path between the given source and destination.
- We using **randomization** to get the current state of all the paths for accidents, traffic and other external conditions that impacts the picking of the path in end.
- It uses Django and DRF(Django REST Framework) for API to give a seamless backend and user experience.
- It stores the history of the searches and the result of it.
- Seamless user experience without any lag.
- Opted for only laptop screen for seamless experience , better to minimize the screen to 90% for better experience.


> It's my creative Application prototype with my custom algorithm (AI Powered)

---

## References

- [A* Algorithm](https://en.wikipedia.org/wiki/A*_search_algorithm) - An AI algorithm (Path Planning Algorithm) is a method that enables machines to perform tasks requiring human-like intelligence, such as learning, pattern recognition, and decision-making.
- [Dijsktra Algorithm](https://en.wikipedia.org/wiki/Dijkstra%27s_algorithm) - Dijkstra's algorithm is a shortest-path algorithm that finds the minimum distance from a starting node to all other nodes in a weighted graph.
- [Django Backend](https://docs.djangoproject.com/en/5.1/) - Backend Python Framework for seamless experience
- [Django REST API](https://www.django-rest-framework.org/) - Django REST Framework to interact with frontend through API calls.
---
## Installation

## Step 1 : Clone the repository / Download the zip of the repository and unzip.

```sh
git clone https://github.com/S-K-Siva/NavGoa-Map.git
```

## Step 1.1 : If unzipped, open the folder in VS Code , Navigate to the folder and follow the below command.

```sh
code .
```
## Step 2 : Create a virtual environment

```sh
virtualenv venv
```

## Step 3 : Activate the virtual environment

```sh
source venv/bin/activate
```

## Step 4 : Download the dependecies of the project

```sh
pip3 install -r requirements.txt
```

## Step 5 : Start the server at the port **8000**

```sh
python3 manage.py runserver 8000
```
---
## Application Interface pics

### Screen 1 - Source and Destination
<img width="721" alt="Screenshot 2024-08-27 at 7 14 32 PM" src="https://github.com/user-attachments/assets/af79fa92-471a-45d6-be64-adbe1fa348cb">


### Screen 2 - Output of the best shortest path at the current situtations

- **Red Pointer** indicates the source and destination
- **Green Pointer** indicates the best shortest path at the current situations
<img width="1440" alt="Screenshot 2024-08-27 at 7 14 17 PM" src="https://github.com/user-attachments/assets/db47aec5-1570-4cc7-84a2-fa955cd53091">


### Screen 3 - History of the searches and it's respective output.
<img width="721" alt="Screenshot 2024-08-27 at 7 14 48 PM" src="https://github.com/user-attachments/assets/3b36b800-e7b6-49ea-945a-c2f0036b7978">

----
# API Endpoints

#### To get all the history of the searches made so far (GET)
```url
http://127.0.0.1:8000/api/
```

#### To get the best shortest path in the current situation (POST)
```url
http://127.0.0.1:8000/api/post
```

---
# Contributors
- **SIVA S K** - AP21110010068

# License
### MIT
