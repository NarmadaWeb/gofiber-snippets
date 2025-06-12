
# Gofiber-Snippets
![Go Fiber](https://img.shields.io/badge/Go-Fiber-00ADD8?style=for-the-badge&logo=go)
![VS Code](https://img.shields.io/badge/Visual_Studio_Code-007ACC?style=for-the-badge&logo=visual-studio-code)
![License](https://img.shields.io/badge/license-MIT-blue?style=for-the-badge)

A comprehensive collection of VS Code snippets to speed up web development with [Go Fiber](https://gofiber.io/). Simply copy the contents of `snippets.json` into your `go.json` file in VS Code.

## How to Use the Snippets
Inside a Go file (`.go`), type one of the prefixes below and press `Tab` or `Enter` to insert the pre-configured code block.

### 🚀 Application Core
| Prefix | Description |
| --- | --- |
| `fiber-init` | Basic Fiber application skeleton with logger and configuration. |
| `fiber-config-env` | Load configuration (like port) from environment variables. |
| `fiber-shutdown` | Implements graceful shutdown to safely terminate the server. |
| `fiber-health` | A `/health` endpoint for status checks and monitoring. |

### 🌐 Routing & Parameters
| Prefix | Description |
| --- | --- |
| `fiber-handler` | Basic skeleton for a route handler (GET, POST, etc.). |
| `fiber-group` | Group routes under a common prefix (e.g., `/api/v1`). |
| `fiber-group-middleware` | Apply middleware to a specific group of routes. |
| `fiber-param` | Get a parameter from the URL path (e.g., `/users/:id`). |
| `fiber-param-optional` | Handle an optional path parameter (e.g., `/users/:name?`). |
| `fiber-param-wildcard` | Capture all paths after a wildcard (e.g., `/files/*`). |
| `fiber-query` | Get query parameters from the URL (e.g., `?page=1&limit=10`). |
| `fiber-redirect` | Redirect a request to another URL with a 301 or 302 status. |

### 📥 Request & Body
| Prefix | Description |
| --- | --- |
| `fiber-body` | Parse a request body (JSON) into a struct. |
| `fiber-body-validation`| Parse and validate a request body using `validator`. |
| `fiber-upload` | Handle a single file upload from a form. |
| `fiber-upload-multi` | Handle multiple file uploads from a single form field. |
| `fiber-header` | Get request headers (e.g., `User-Agent`, `Authorization`). |

### 📤 Response & Data
| Prefix | Description |
| --- | --- |
| `fiber-json` | Create a standardized JSON response (`success`, `message`, `data`). |
| `fiber-static` | Serve static files like HTML, CSS, and JS from a directory. |
| `fiber-template-html` | Configure and render an HTML template. |
| `fiber-download` | Serve a file for a client to download. |
| `fiber-cookie` | Set, get, and clear cookies. |

### 🛡️ Middleware
| Prefix | Description |
| --- | --- |
| `fiber-middleware` | Basic structure for creating your own custom middleware. |
| `fiber-error` | Global middleware to handle all errors centrally. |
| `fiber-middleware-recover` | The `Recover` middleware to catch panics and keep the server running. |
| `fiber-middleware-requestid`| The `RequestID` middleware to add a unique ID to each request. |
| `fiber-middleware-compress` | The `Compress` middleware to compress responses (gzip, brotli). |
| `fiber-cors` | Configure Cross-Origin Resource Sharing (CORS). |
| `fiber-limit` | The `Limiter` middleware for rate limiting requests. |
| `fiber-middleware-next-locals`| Pass data from a middleware to a handler using `c.Locals()`. |

### 🔐 Authentication (JWT)
| Prefix | Description |
| --- | --- |
| `fiber-jwt` | JWT middleware to protect routes with token authentication. |
| `fiber-jwt-generate` | Generate a new JWT token with custom claims. |
| `fiber-jwt-getuser` | Get user data (claims) from a JWT token inside a handler. |

### 🗃️ Database (GORM)
| Prefix | Description |
| --- | --- |
| `fiber-db` | Connect to a database (GORM) and inject it into the context. |
| `fiber-db-use` | Get the database connection from the context inside a handler. |

### 📡 Real-time Communication
| Prefix | Description |
| --- | --- |
| `fiber-ws` | Basic skeleton for a WebSocket server. |
| `fiber-sse` | Create an endpoint for Server-Sent Events (SSE). |

### 🧪 Testing
| Prefix | Description |
| --- | --- |
| `fiber-test-handler`| Template for a unit test of a Fiber handler using `httptest`. |

## License

This project is licensed under the MIT License.
