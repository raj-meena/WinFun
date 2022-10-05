<template>
    <footer>
        <nav>
            <RouterLink to="/">
                <svg
                    id="home"
                    xmlns="http://www.w3.org/2000/svg"
                    width="27.086"
                    height="24"
                    viewBox="0 0 27.086 24"
                >
                    <path
                        id="Path_9"
                        data-name="Path 9"
                        d="M3.588,24.3a.553.553,0,0,0,.573.59l6.9-.008.01-5.451a.78.78,0,0,1,.806-.9h2.863c1.069,0,1,.9,1,.9l-.012,5.434H22.48a.689.689,0,0,0,.725-.734V14.076L13.689,5.913l-10.1,8.164S3.588,24.3,3.588,24.3Z"
                        transform="translate(0 -0.887)"
                    />
                    <path
                        id="Path_10"
                        data-name="Path 10"
                        d="M0,13.317s.848,1.524,2.7,0L13.766,4.2,24.14,13.26c2.143,1.506,2.947,0,2.947,0L13.766,1.5Z"
                        transform="translate(0 -1.504)"
                    />
                    <path
                        id="Path_11"
                        data-name="Path 11"
                        d="M23.273,4.175h-2.6l.011,3.153,2.588,2.2Z"
                        transform="translate(0.696 -1.504)"
                    />
                </svg>

                <span>Home</span>
            </RouterLink>
            <RouterLink to="/search">
                <svg
                    xmlns="http://www.w3.org/2000/svg"
                    width="20.314"
                    height="20.315"
                    viewBox="0 0 20.314 20.315"
                >
                    <g id="search" transform="translate(-2 -1.999)">
                        <path
                            id="Path_5"
                            data-name="Path 5"
                            d="M18.031,16.617,22.314,20.9,20.9,22.314l-4.282-4.283a9,9,0,1,1,1.414-1.414Zm-2.006-.742a7,7,0,1,0-.15.15l.15-.15Z"
                        />
                    </g>
                </svg>

                <span>Search</span>
            </RouterLink>
            <RouterLink to="/dashboard">
                <svg
                    xmlns="http://www.w3.org/2000/svg"
                    width="24.333"
                    height="24"
                    viewBox="0 0 24.333 24"
                >
                    <g id="trophy" transform="translate(0 -1)">
                        <rect
                            id="trophy-2"
                            data-name="trophy"
                            width="12"
                            height="1"
                            transform="translate(6 24)"
                        />
                        <path
                            id="trophy-3"
                            data-name="trophy"
                            d="M19.984,3.791,20.54,1H3.793l.556,2.791H0V4.836a10.043,10.043,0,0,0,2.1,6.182,10.216,10.216,0,0,0,5.023,3.5,6.538,6.538,0,0,0,3.988,2.554v2.362H7.374v2.633h9.533V19.434H13.22V17.072a6.537,6.537,0,0,0,3.992-2.555,10.216,10.216,0,0,0,5.018-3.5,10.043,10.043,0,0,0,2.1-6.182V3.791ZM2.176,5.9H4.77l1.156,5.784A8.143,8.143,0,0,1,2.176,5.9Zm9.99,9.691v-1.58a3.393,3.393,0,0,0,3.053-2.5l1.538.363A4.94,4.94,0,0,1,12.167,15.589Zm6.241-3.908L19.563,5.9h2.593A8.142,8.142,0,0,1,18.408,11.682Z"
                        />
                    </g>
                </svg>

                <span>Dashboard</span>
            </RouterLink>
            <RouterLink to="/account">
                <svg
                    xmlns="http://www.w3.org/2000/svg"
                    width="24.496"
                    height="24"
                    viewBox="0 0 24.496 24"
                >
                    <path
                        id="profile"
                        d="M28.023,25.7a12.924,12.924,0,0,0-5.948-7.068,8.673,8.673,0,1,0-12.6,0A12.924,12.924,0,0,0,3.527,25.7,15.994,15.994,0,0,0,5.883,28a10.068,10.068,0,0,1,6.834-7.625,1.445,1.445,0,0,0,.262-2.644,5.782,5.782,0,1,1,5.6,0,1.445,1.445,0,0,0,.262,2.644A10.068,10.068,0,0,1,25.667,28,15.986,15.986,0,0,0,28.023,25.7Z"
                        transform="translate(-3.527 -3.999)"
                    />
                </svg>

                <span>My Account</span>
            </RouterLink>
        </nav>
    </footer>
</template>

<style scoped>
footer {
    width: 100%;
    height: 50px;
    background: #fff;
    position: fixed;
    bottom: 0;
    left: 0;
    display: flex;
    justify-content: center;
    align-items: center;
    box-shadow: 0 3px 14px 2px rgba(0, 0, 0, 0.12);
}
nav {
    width: 100%;
    display: flex;
    flex-direction: row;
    justify-content: space-between;
}
nav a {
    width: 25%;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    color: #000;
    text-decoration: none;
    padding-top: 3px;
}
nav a svg {
    height: 20px;
}
nav a span {
    font-size: 12px;
    margin-top: 3px;
    line-height: 18px;
    display: block;
}
nav a.router-link-exact-active span {
    color: #f81f01;
}
nav a.router-link-exact-active svg path {
    fill: #ee076e;
}
</style>
