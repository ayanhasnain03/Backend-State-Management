<h1>Docker Guide 🐳 Level 1</h1>
<a>https://guide-note-app.vercel.app/blog/docker-level-1</a>

<p>This README provides an overview of why we need Docker, where to get Docker images, and a collection of common commands to help you navigate Docker from basic to advanced operations. Keep this handy as you work with Docker! 🚀</p>

<hr>

<h2>Why We Need Docker</h2>
<ul>
    <li><strong>Consistent Environment</strong>: Ensures your app runs the same way everywhere, whether on your laptop or a server, by packaging everything it needs (like code, libraries, etc.) into a container.</li>
    <li><strong>Easy Setup</strong>: Quickly set up and run apps without worrying about installation issues (e.g., missing dependencies).</li>
    <li><strong>Isolation</strong>: Each app runs in its own container, so if one app crashes, others remain unaffected.</li>
    <li><strong>Scalability</strong>: Easily scale your apps up or down based on demand by creating more container instances.</li>
    <li><strong>Efficiency</strong>: Uses fewer resources than virtual machines (VMs) because containers share the same operating system, making them lightweight.</li>
</ul>

<hr>

<h2>Where Can We Get Packages From?</h2>
<p>Just like you can push your code to GitHub/GitLab, you can push images to Docker registries.</p>

<h3>Docker Hub</h3>
<p>The main public repository for Docker images. You can find a wide variety of pre-built images for popular software like Node.js, MongoDB, PostgreSQL, etc. Simply pull an image using:</p>
<pre><code>docker pull &lt;image-name&gt;</code></pre>
<p>Example:</p>
<pre><code>docker pull node</code></pre>

<h3>Private Repository</h3>
<p>If you're working in a company, you might store Docker images in a private repository. Docker Hub allows private repositories, or you can use alternatives like:</p>
<ul>
    <li><strong>AWS Elastic Container Registry (ECR)</strong></li>
    <li><strong>Google Container Registry (GCR)</strong></li>
    <li><strong>Azure Container Registry (ACR)</strong></li>
</ul>

<h3>Building Your Own</h3>
<p>You can create your own Docker image using a <code>Dockerfile</code> that specifies the dependencies and setup for your app. Build the image with:</p>
<pre><code>docker build -t &lt;your-image-name&gt; .</code></pre>

<h3>GitHub Packages</h3>
<p>You can store Docker images in GitHub's package registry, useful for integrating with your CI/CD workflows.</p>

<hr>

<h2>Common Commands to Know 🔥</h2>

<h3>📦 Image Commands</h3>
<ul>
    <li><strong>Pull an image from Docker Hub:</strong>
        <pre><code>docker pull &lt;image-name&gt;</code></pre>
        Example: 
        <pre><code>docker pull node</code></pre>
    </li>
    <li><strong>List all downloaded images:</strong>
        <pre><code>docker images</code></pre>
    </li>
    <li><strong>Remove an image:</strong>
        <pre><code>docker rmi &lt;image-id&gt;</code></pre>
    </li>
</ul>

<h3>🐳 Container Commands</h3>
<ul>
    <li><strong>Run a new container (detached mode):</strong>
        <pre><code>docker run -d --name &lt;container-name&gt; &lt;image-name&gt;</code></pre>
        Example:
        <pre><code>docker run -d --name my-app node</code></pre>
    </li>
    <li><strong>List all running containers:</strong>
        <pre><code>docker ps</code></pre>
    </li>
    <li><strong>List all containers (including stopped):</strong>
        <pre><code>docker ps -a</code></pre>
    </li>
    <li><strong>Stop a running container:</strong>
        <pre><code>docker stop &lt;container-name&gt;</code></pre>
    </li>
    <li><strong>Remove a container:</strong>
        <pre><code>docker rm &lt;container-name&gt;</code></pre>
    </li>
    <li><strong>Restart a stopped container:</strong>
        <pre><code>docker start &lt;container-name&gt;</code></pre>
    </li>
</ul>

<h3>🛠 Docker Exec Commands</h3>
<ul>
    <li><strong>Enter a running container's shell:</strong>
        <pre><code>docker exec -it &lt;container-name&gt; /bin/bash</code></pre>
    </li>
</ul>

<hr>

<p>These commands will help you navigate Docker from basic usage to more advanced operations. Keep this cheat sheet handy as you work with Docker! Happy coding! 🚀</p>

<h2>More on Docker Level 2 🌟</h2>
<p>Explore more advanced topics and best practices in Docker for deeper insights and efficient workflows.</p>
