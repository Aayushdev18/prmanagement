**POSTMAN JSON COLLECTIONS TO CHECK All the endpoints**
`{
	"info": {
		"_postman_id": "3d6775e9-d129-475c-84a7-30aae2057101",
		"name": "Project Management System",
		"schema": "https://schema.getpostman.com/json/collection/v2.1.0/collection.json",
		"_exporter_id": "33683810",
		"_collection_link": "https://bold-satellite-536738.postman.co/workspace/New-Team-Workspace~23f8d1f0-c587-49b8-9800-8289f7e42eb9/collection/33683810-3d6775e9-d129-475c-84a7-30aae2057101?action=share&source=collection_link&creator=33683810"
	},
	"item": [
		{
			"name": "POST Signup",
			"request": {
				"method": "POST",
				"header": [
					{
						"key": "Content-Type",
						"value": "application/json",
						"type": "text"
					}
				],
				"body": {
					"mode": "raw",
					"raw": "{\n    \"email\":\"aran@gmail.com\",\n    \"username\":\"aryanovescode\",\n    \"password\":\"Aryan@123\"\n}",
					"options": {
						"raw": {
							"language": "json"
						}
					}
				},
				"url": {
					"raw": "https://project-management-system-dig0.onrender.com/api/user/signup",
					"protocol": "https",
					"host": [
						"project-management-system-dig0",
						"onrender",
						"com"
					],
					"path": [
						"api",
						"user",
						"signup"
					]
				}
			},
			"response": []
		},
		{
			"name": "POST Login",
			"request": {
				"method": "POST",
				"header": [
					{
						"key": "Content-Type",
						"value": "application/json",
						"type": "text"
					}
				],
				"body": {
					"mode": "raw",
					"raw": "{\n    \"email\":\"haryan458@gmail.com\",\n    \"password\":\"haryan458@gmail.com\"\n}",
					"options": {
						"raw": {
							"language": "json"
						}
					}
				},
				"url": {
					"raw": "https://project-management-system-dig0.onrender.com/api/users/login",
					"protocol": "https",
					"host": [
						"project-management-system-dig0",
						"onrender",
						"com"
					],
					"path": [
						"api",
						"users",
						"login"
					]
				}
			},
			"response": []
		},
		{
			"name": "POST Create Project",
			"request": {
				"auth": {
					"type": "bearer",
					"bearer": [
						{
							"key": "token",
							"value": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ1c2VySWQiOjEsImlhdCI6MTczMDU2Mjc2NCwiZXhwIjoxNzMwNTY2MzY0fQ.wFyay3ibUy4FYCTEkdBBnXYIep-8ZU8XqurW-u3E4g8",
							"type": "string"
						}
					]
				},
				"method": "POST",
				"header": [
					{
						"key": "Authorization",
						"value": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ1c2VySWQiOjEsImlhdCI6MTcyODA3MjIyMywiZXhwIjoxNzI4MDc1ODIzfQ.6y3XmMdoEw87W63puj7dpQ9TsPHxOhf6oj4GxmnWVqw",
						"type": "text"
					}
				],
				"body": {
					"mode": "raw",
					"raw": "{\n    \"name\":\"Project 19\",\n    \"description\":\"Pro description\"\n}",
					"options": {
						"raw": {
							"language": "json"
						}
					}
				},
				"url": {
					"raw": "https://project-management-system-dig0.onrender.com/api/projects/create",
					"protocol": "https",
					"host": [
						"project-management-system-dig0",
						"onrender",
						"com"
					],
					"path": [
						"api",
						"projects",
						"create"
					]
				}
			},
			"response": []
		},
		{
			"name": "POST Create Task",
			"request": {
				"auth": {
					"type": "bearer",
					"bearer": [
						{
							"key": "token",
							"value": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ1c2VySWQiOjEsImlhdCI6MTcyODA3OTE0MCwiZXhwIjoxNzI4MDgyNzQwfQ.wtXN6aYkkwBV_6VydclqaCgCk3ua0BueKlQg8OSOXlA",
							"type": "string"
						}
					]
				},
				"method": "POST",
				"header": [
					{
						"key": "Authorization",
						"value": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ1c2VySWQiOjEsImlhdCI6MTcyODA3OTE0MCwiZXhwIjoxNzI4MDgyNzQwfQ.wtXN6aYkkwBV_6VydclqaCgCk3ua0BueKlQg8OSOXlA",
						"type": "text"
					}
				],
				"body": {
					"mode": "raw",
					"raw": "{\n    \"title\":\"task14\",\n    \"description\":\"Description for task\",\n    \"projectId\":16\n}",
					"options": {
						"raw": {
							"language": "json"
						}
					}
				},
				"url": {
					"raw": "https://project-management-system-dig0.onrender.com/api/task/create",
					"protocol": "https",
					"host": [
						"project-management-system-dig0",
						"onrender",
						"com"
					],
					"path": [
						"api",
						"task",
						"create"
					]
				}
			},
			"response": []
		},
		{
			"name": "DELETE Delete a task",
			"request": {
				"auth": {
					"type": "bearer",
					"bearer": [
						{
							"key": "token",
							"value": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ1c2VySWQiOjEsImlhdCI6MTcyNzU3MDE3NiwiZXhwIjoxNzI3NTczNzc2fQ.UDSHULsB7_evVboC7bX0bUxNwSHJvtMsIXxGJ_K6QGg",
							"type": "string"
						}
					]
				},
				"method": "DELETE",
				"header": [
					{
						"key": "Authorization",
						"value": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ1c2VySWQiOjEsImlhdCI6MTcyNzU3MDE3NiwiZXhwIjoxNzI3NTczNzc2fQ.UDSHULsB7_evVboC7bX0bUxNwSHJvtMsIXxGJ_K6QGg",
						"type": "text"
					}
				],
				"url": {
					"raw": "https://project-management-system-dig0.onrender.com/api/task/delete/1",
					"protocol": "https",
					"host": [
						"project-management-system-dig0",
						"onrender",
						"com"
					],
					"path": [
						"api",
						"task",
						"delete",
						"1"
					]
				}
			},
			"response": []
		},
		{
			"name": "Update task",
			"request": {
				"auth": {
					"type": "bearer",
					"bearer": [
						{
							"key": "token",
							"value": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ1c2VySWQiOjIsImlhdCI6MTcyODY3MjkyMiwiZXhwIjoxNzI4Njc2NTIyfQ.aPExOYQ2rC7JPSwBzLb3c_TPY7OP3zuO8QP8svcrVlk",
							"type": "string"
						}
					]
				},
				"method": "POST",
				"header": [
					{
						"key": "Authorization",
						"value": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ1c2VySWQiOjIsImlhdCI6MTcyODU0NDM5MSwiZXhwIjoxNzI4NTQ3OTkxfQ.JvH_-SLLce-Qm-Uti1ZL141B9BCLsDVay9BYwdfLCe0",
						"type": "text"
					}
				],
				"body": {
					"mode": "raw",
					"raw": "{\n    \"name\":\"user1\",\n    \"email\":\"user1@gmail.com\",\n    \"password\":\"12345678\"\n}",
					"options": {
						"raw": {
							"language": "json"
						}
					}
				},
				"url": {
					"raw": "https://project-management-system-dig0.onrender.com/api/voter/auth/signup",
					"protocol": "https",
					"host": [
						"project-management-system-dig0",
						"onrender",
						"com"
					],
					"path": [
						"api",
						"voter",
						"auth",
						"signup"
					]
				}
			},
			"response": []
		},
		{
			"name": "GET a task",
			"request": {
				"auth": {
					"type": "bearer",
					"bearer": [
						{
							"key": "token",
							"value": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ1c2VySWQiOjEsImlhdCI6MTcyNzU3MDE3NiwiZXhwIjoxNzI3NTczNzc2fQ.UDSHULsB7_evVboC7bX0bUxNwSHJvtMsIXxGJ_K6QGg",
							"type": "string"
						}
					]
				},
				"method": "GET",
				"header": [
					{
						"key": "Authorization",
						"value": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ1c2VySWQiOjEsImlhdCI6MTcyNzU3MDE3NiwiZXhwIjoxNzI3NTczNzc2fQ.UDSHULsB7_evVboC7bX0bUxNwSHJvtMsIXxGJ_K6QGg",
						"type": "text"
					}
				],
				"url": {
					"raw": "https://project-management-system-dig0.onrender.com/api/task/2",
					"protocol": "https",
					"host": [
						"project-management-system-dig0",
						"onrender",
						"com"
					],
					"path": [
						"api",
						"task",
						"2"
					]
				}
			},
			"response": []
		},
		{
			"name": "GET ALL tasks",
			"request": {
				"auth": {
					"type": "bearer",
					"bearer": [
						{
							"key": "token",
							"value": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ1c2VySWQiOjIsImlhdCI6MTcyODY3MjkyMiwiZXhwIjoxNzI4Njc2NTIyfQ.aPExOYQ2rC7JPSwBzLb3c_TPY7OP3zuO8QP8svcrVlk",
							"type": "string"
						}
					]
				},
				"method": "GET",
				"header": [
					{
						"key": "Authorization",
						"value": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ1c2VySWQiOjIsImlhdCI6MTcyODY3MjkyMiwiZXhwIjoxNzI4Njc2NTIyfQ.aPExOYQ2rC7JPSwBzLb3c_TPY7OP3zuO8QP8svcrVlk",
						"type": "text"
					}
				],
				"url": {
					"raw": "https://project-management-system-dig0.onrender.com/api/task",
					"protocol": "https",
					"host": [
						"project-management-system-dig0",
						"onrender",
						"com"
					],
					"path": [
						"api",
						"task"
					]
				}
			},
			"response": []
		},
		{
			"name": "Get Task associated with project",
			"request": {
				"auth": {
					"type": "bearer",
					"bearer": [
						{
							"key": "token",
							"value": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ1c2VySWQiOjEsImlhdCI6MTcyODE1OTYwOCwiZXhwIjoxNzI4MTYzMjA4fQ.ADIdHm5-d7xGmRPBCJX1GgjsqTM7BL2y67RdhSWo1Ik",
							"type": "string"
						}
					]
				},
				"method": "GET",
				"header": [
					{
						"key": "Authorization",
						"value": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ1c2VySWQiOjEsImlhdCI6MTcyNzU3MDE3NiwiZXhwIjoxNzI3NTczNzc2fQ.UDSHULsB7_evVboC7bX0bUxNwSHJvtMsIXxGJ_K6QGg",
						"type": "text"
					}
				],
				"url": {
					"raw": "https://project-management-system-dig0.onrender.com/api/task/project",
					"protocol": "https",
					"host": [
						"project-management-system-dig0",
						"onrender",
						"com"
					],
					"path": [
						"api",
						"task",
						"project"
					]
				}
			},
			"response": []
		}
	]
}`