# Homework1_zoomcamp
Solutions for Homework 1


## Question 1. Knowing docker tags

Run the command to get information on Docker 

```docker --help```

Now run the command to get help on the "docker build" command:

```docker build --help```

Do the same for "docker run".

Which tag has the following text? - *Automatically remove the container when it exits* 

- `--delete`
- `--rc`
- `--rmc`
- `--rm`

After running the command

```docker run --help```

We can see in the picture that the answer is

- `--rm`

<img src="https://github.com/juandavidlozano/Homework1_zoomcamp/blob/main/homework1.1.jpg" alt="Answer 1" width="1000" height="900">




## Question 2. Understanding docker first run 

Run docker with the python:3.9 image in an interactive mode and the entrypoint of bash.
Now check the python modules that are installed ( use ```pip list``` ). 

What is version of the package *wheel* ?

- 0.42.0
- 1.0.0
- 23.0.1
- 58.1.0


We can see in the picture that the answer is 


- 0.42.0


<img src="https://github.com/juandavidlozano/Homework1_zoomcamp/blob/main/homework1.2.jpg" alt="Answer 1" width="1000" height="500">




## Question 3. Count records 

How many taxi trips were totally made on September 18th 2019?

Tip: started and finished on 2019-09-18. 

Remember that `lpep_pickup_datetime` and `lpep_dropoff_datetime` columns are in the format timestamp (date and hour+min+sec) and not in date.

- 15767
- 15612
- 15859
- 89009


we can see in the picture the answer is 15612


<img src="https://github.com/juandavidlozano/Homework1_zoomcamp/blob/main/homework1.3.jpg" alt="Answer 1" width="1000" height="500">



