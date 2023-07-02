
# Job Search Application

The Job Search Application is a RESTful API that provides endpoints to manage job search data. It allows users to retrieve, create, update, and delete job search entries.

## Technologies Used

- Java
- Spring Boot
- Spring Data JPA
- Spring Web
- MySQL (H2 DATABASE)
- Maven 

## Prerequisites

- Java 8 or higher installed
- Database setup (MySQL or other supported database)
- IDE (e.g., IntelliJ IDEA, Eclipse)

## Getting Started

1. Clone the repository:

   ```bash
   git clone https://github.com/your-username/job-search-application.git](https://github.com/Sanowar72/job-serach/tree/main)




## API Endpoints

### Get All Jobs

- Endpoint: `GET /all`
- Description: Retrieves all job search entries.
- Response: Array of job search entries.

### Save All Jobs

- Endpoint: `POST /save-all`
- Description: Saves multiple job search entries.
- Request Body: Array of job search entries.
- Response: Success message.

### Find Jobs by Job Title

- Endpoint: `GET /job-title/{jobtitle}`
- Description: Finds job search entries by job title.
- Path Parameter:
  - `jobtitle` - Job title to search for.
- Response: Array of job search entries with matching job titles.

### Find Jobs by Job Location

- Endpoint: `GET /job-location/{location}`
- Description: Finds job search entries by job location.
- Path Parameter:
  - `location` - Job location to search for.
- Response: Array of job search entries with matching job locations.

### Find Jobs by Employer Name

- Endpoint: `GET /employer-name/{name}`
- Description: Finds job search entries by employer name.
- Path Parameter:
  - `name` - Employer name to search for.
- Response: Array of job search entries with matching employer names.

### Update Job Salary by ID

- Endpoint: `PUT /byid/{id}/{salary}`
- Description: Updates the salary of a job search entry by its ID.
- Path Parameters:
  - `id` - ID of the job search entry.
  - `salary` - New salary value.
- Response: Success message.

### Delete Job by ID

- Endpoint: `DELETE /byid/{id}`
- Description: Deletes a job search entry by its ID.
- Path Parameter:
  - `id` - ID of the job search entry.
- Response: Success message.
## Validation

The Job Search Application includes the following validations:

- Email Validation: The `companyEmail` field of a job search entry must be a valid email format.

- Minimum Salary Validation: The `jobSalary` field of a job search entry must be greater than or equal to 20,000.

These validations ensure the data integrity and consistency of the job search entries.
