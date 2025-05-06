# PocketBase on Gitpod

This repository sets up a **PocketBase** instance hosted on **Gitpod**, providing a lightweight, self-hosted backend-as-a-service with a real-time database, authentication, file storage, and an admin dashboard. With just a few clicks, you can spin up a fully functional PocketBase server in the cloud using Gitpod's development environment.

## Features
- **PocketBase**: A Go-based backend with SQLite, offering REST API, real-time subscriptions, and file management.
- **Gitpod Integration**: Automated setup via `.gitpod.yml` for instant deployment.
- **Accessible Admin UI**: Access the PocketBase admin dashboard via Gitpod's preview URL on port 8090.
- **Portable & Reproducible**: Fork the repo, open in Gitpod, and have a running backend in seconds.

## Prerequisites
- A GitHub account.
- Access to [Gitpod](https://gitpod.io/) (free tier is sufficient for this setup).
- Basic familiarity with PocketBase and Gitpod.

## Getting Started

### 1. Fork the Repository
To use or modify this PocketBase setup:
- Go to the [repository page](https://github.com/aklavya20/pocketbase).
- Click the **Fork** button in the top-right corner to create a copy under your GitHub account.

Replace `YOUR_USERNAME/YOUR_REPOSITORY` with the actual GitHub username and repository name.

### 2. Open in Gitpod
Launch the forked repository in Gitpod:
- Navigate to your forked repo (e.g., `https://github.com/YOUR_USERNAME/YOUR_REPOSITORY`).
- Prepend `https://gitpod.io/#` to the repo URL, like this:
  ```
  https://gitpod.io/#https://github.com/YOUR_USERNAME/YOUR_REPOSITORY
  ```
- Open the URL in a browser, or use the button below if added to the repo:

  [![Open in Gitpod](https://gitpod.io/button/open-in-gitpod.svg)](https://gitpod.io/#https://github.com/aklavya20/https://github.com/aklavya20/pocketbase.git)

- Gitpod will set up the workspace, start the PocketBase server, and open a preview on port `8090`.

### 3. Access the Admin Dashboard
- In the Gitpod workspace, the preview window will show the PocketBase admin UI at `http://localhost:8090`.
- Create an admin account by following the prompts to set an email and password.
- Log in to manage collections, users, and files.

### 4. Use the API
Interact with PocketBase via:
- REST API at `http://localhost:8090/api/` using tools like cURL or Postman.
- [PocketBase JS SDK](https://pocketbase.io/docs/client-side) for frontend apps.
- [PocketBase Go SDK](https://pocketbase.io/docs/server-side) for server-side integration.

See the [PocketBase documentation](https://pocketbase.io/docs/) for more details.

## Project Structure
```
├── pocketbase       # PocketBase Linux executable
├── .gitpod.yml      # Gitpod configuration file
└── README.md        # This file
```

## Notes
- **Data Persistence**: Data is stored in SQLite within the Gitpod workspace. If the workspace is deleted, data may be lost. For persistent storage, consider external database solutions or manual backups.
- **Customizations**: Extend PocketBase with custom routes or logic by adding JavaScript or Go code (see [PocketBase docs](https://pocketbase.io/docs/)).
- **Security**: The admin dashboard is publicly accessible in Gitpod’s preview. Secure your instance by setting strong admin credentials and restricting access if needed.

## Contributing
Contributions are welcome! To contribute:
1. Fork this repository.
2. Create a new branch (`git checkout -b feature/your-feature`).
3. Commit your changes (`git commit -m "Add your feature"`).
4. Push to the branch (`git push origin feature/your-feature`).
5. Open a pull request.

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Acknowledgments
- [PocketBase](https://pocketbase.io/) for the awesome backend framework.
- [Gitpod](https://gitpod.io/) for the cloud development environment.

Happy coding! 🚀
