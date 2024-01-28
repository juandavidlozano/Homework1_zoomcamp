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



## Question 4. Largest trip for each day

Which was the pick up day with the largest trip distance
Use the pick up time for your calculations.

- 2019-09-18
- 2019-09-16
- 2019-09-26
- 2019-09-21

We can see from the picture that it was on 2019-09-26




<img src="https://github.com/juandavidlozano/Homework1_zoomcamp/blob/main/homework1.4.jpg" alt="Answer 1" width="1000" height="500">




## Question 5. Three biggest pick up Boroughs

Consider lpep_pickup_datetime in '2019-09-18' and ignoring Borough has Unknown

Which were the 3 pick up Boroughs that had a sum of total_amount superior to 50000?
 
- "Brooklyn" "Manhattan" "Queens"
- "Bronx" "Brooklyn" "Manhattan"
- "Bronx" "Manhattan" "Queens" 
- "Brooklyn" "Queens" "Staten Island"


we can see in the picture that the answer is


- "Brooklyn" "Manhattan" "Queens"


<img src="https://github.com/juandavidlozano/Homework1_zoomcamp/blob/main/homework1.5.jpg" alt="Answer 1" width="1000" height="500">


## Question 6. Largest tip

For the passengers picked up in September 2019 in the zone name Astoria which was the drop off zone that had the largest tip?
We want the name of the zone, not the id.

Note: it's not a typo, it's `tip` , not `trip`

- Central Park
- Jamaica
- JFK Airport
- Long Island City/Queens Plaza


we can see from the picture that the answer is

- JFK Airport


<img src="https://github.com/juandavidlozano/Homework1_zoomcamp/blob/main/homework1.6.jpg" alt="Answer 1" width="1000" height="500">



## Question 7. Creating Resources

After updating the main.tf and variable.tf files run:

```
terraform apply
```

Paste the output of this command into the homework submission form.


this was my output

(base) juand@de-zoomcamp:~/data-engineering-zoomcamp/01-docker-terraform/1_terraform_gcp/terraform/terraform_with_variables$ terraform apply
google_bigquery_dataset.demo_dataset: Refreshing state... [id=projects/test-402517/datasets/demo_dataset]

Terraform used the selected providers to generate the following execution plan. Resource actions are indicated with the following
symbols:
  + create

Terraform will perform the following actions:

  # google_storage_bucket.demo-bucket will be created
  + resource "google_storage_bucket" "demo-bucket" {
      + effective_labels            = (known after apply)
      + force_destroy               = true
      + id                          = (known after apply)
      + location                    = "US"
      + name                        = "juan-lozano-terraform-demo-terra-bucket"
      + project                     = (known after apply)
      + public_access_prevention    = (known after apply)
      + self_link                   = (known after apply)
      + storage_class               = "STANDARD"
      + terraform_labels            = (known after apply)
      + uniform_bucket_level_access = (known after apply)
      + url                         = (known after apply)

      + lifecycle_rule {
          + action {
              + type = "AbortIncompleteMultipartUpload"
            }
          + condition {
              + age                   = 1
              + matches_prefix        = []
              + matches_storage_class = []
              + matches_suffix        = []
              + with_state            = (known after apply)
            }
        }
    }

Plan: 1 to add, 0 to change, 0 to destroy.

Do you want to perform these actions?
  Terraform will perform the actions described above.
  Only 'yes' will be accepted to approve.

  Enter a value: yes

google_storage_bucket.demo-bucket: Creating...
google_storage_bucket.demo-bucket: Creation complete after 1s [id=juan-lozano-terraform-demo-terra-bucket]

Apply complete! Resources: 1 added, 0 changed, 0 destroyed.


















