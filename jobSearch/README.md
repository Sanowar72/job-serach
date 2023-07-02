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