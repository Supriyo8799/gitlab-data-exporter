# GitLab Data Exporter

A tool to export GitLab user's starred projects, followers, and following as CSV files in a ZIP archive.

## Features

- **Export Starred Projects**: Fetch and export a list of projects a user has starred on GitLab.
- **Export Followers**: Get a list of followers of a GitLab user.
- **Export Following**: Export a list of users that the GitLab user is following.

> **Note**: This tool only lists the **starred projects**, **followers**, and **following** of a GitLab user. It does not include other data such as project details or code from repositories.

## How to Use

1. Enter your **GitLab user ID** and **GitLab Personal Access Token**.
2. Click **Get Data** to fetch the GitLab data (starred projects, followers, following).
3. After data is fetched, a **Download CSV Files** button will appear.
4. Click **Download CSV Files** to download a ZIP archive containing:
   - `gitlab_starredprojects_<username>.csv` (Starred projects)
   - `gitlab_followers_<username>.csv` (Followers list)
   - `gitlab_following_<username>.csv` (Following list)

## How to Get a GitLab Personal Access Token

1. Go to [GitLab Personal Access Tokens](https://gitlab.com/-/profile/personal_access_tokens).
2. Click **Generate New Token**.
3. Select the following **scopes**:
   - **`api`**: Grants full access to the GitLab API, including reading and writing data.
   - **`read_user`**: Grants access to public and private user data, including followers and following. This scope is required to get the followers and following data.
4. Click **Generate Token** and copy it.
5. Paste the token into the input field in the app.

> **Warning**: Please ensure that you do not share your **GitLab Personal Access Token** with others. It provides access to sensitive data and should be kept private. Treat it like a password.

## Tools Used

- **HTML**: The core structure of the application is built using HTML.
- **CSS**: Used for styling and layout of the exporter.
- **JavaScript**: Used for the interactivity and functionality of the exporter.
- **JSZip**: A library to generate the ZIP archive of CSV files for download.
- **GitLab API**: Used to fetch data from GitLab.

## License

This project is licensed under the **No License**.

## Contributing

1. Fork the repository.
2. Create a new branch (`git checkout -b feature/feature-name`).
3. Commit your changes (`git commit -am 'Add new feature'`).
4. Push to the branch (`git push origin feature/feature-name`).
5. Create a new pull request.

## Contact

For any issues or feature requests, please open an issue in the repository.
