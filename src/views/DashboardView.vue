<template>
    <HeaderItem />
    <main class="main">
        <section class="section">
            <ul class="main_nav">
                <li
                    :class="[tabOpen === 1 ? 'active' : '', '']"
                    @click="tab(1)"
                >
                    Sapre
                </li>
                <li
                    :class="[tabOpen === 2 ? 'active' : '', '']"
                    @click="tab(2)"
                >
                    Emerd
                </li>
            </ul>
            <div class="center_text">
                <ul class="center_top">
                    <li class="left_li">
                        <ol class="top_ol">
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
                            <span>Period</span>
                        </ol>
                        <ol class="bot_ol">
                            20221004302
                        </ol>
                    </li>
                    <li class="right_li">
                        <ol class="top_ol">
                            <span>Count Down</span>
                        </ol>
                        <ol class="bot_ol">
                            <div class="countdown">
                                <div class="van-count-down">
                                    <span class="span">0</span
                                    ><span class="span">1</span><span>:</span>
                                    <p>
                                        <span class="span"> 2 </span
                                        ><span class="span"> 9 </span>
                                    </p>
                                </div>
                            </div>
                            <div class="ol_btn" style="display: none">
                                <button class="grayback">Continue</button>
                            </div>
                        </ol>
                    </li>
                </ul>
                <div class="btn_center">
                    <button class="back_one" @click="isShow = !isShow">
                        Join Green</button
                    ><button class="back_two" @click="isShow = !isShow">
                        Join Violet</button
                    ><button class="back_three" @click="isShow = !isShow">
                        Join Red
                    </button>
                </div>
                <ul class="center_notes">
                    <li>
                        <ol class="">
                            0
                        </ol>
                    </li>
                    <li>
                        <ol class="">
                            1
                        </ol>
                    </li>
                    <li>
                        <ol class="">
                            2
                        </ol>
                    </li>
                    <li>
                        <ol class="">
                            3
                        </ol>
                    </li>
                    <li>
                        <ol class="">
                            4
                        </ol>
                    </li>
                    <li>
                        <ol class="">
                            5
                        </ol>
                    </li>
                    <li>
                        <ol class="">
                            6
                        </ol>
                    </li>
                    <li>
                        <ol class="">
                            7
                        </ol>
                    </li>
                    <li>
                        <ol class="">
                            8
                        </ol>
                    </li>
                    <li>
                        <ol class="">
                            9
                        </ol>
                    </li>
                </ul>
            </div>
            <div class="nav_content">
                <div class="content" v-if="tabOpen === 1">
                    <div class="content_con">
                        <div class="content_title">
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
                            <p>Sapre Record</p>
                        </div>
                        <div class="parity">
                            <table>
                                <thead>
                                    <tr>
                                        <th>Period</th>
                                        <th>Price</th>
                                        <th>Number</th>
                                        <th>Result</th>
                                    </tr>
                                    <tr
                                        style="
                                            border: 0px;
                                            width: 100%;
                                            display: none;
                                        "
                                    >
                                        <th
                                            colspan="4"
                                            style="height: 0px; line-height: 0"
                                        >
                                            <div class="table_loading">
                                                <div
                                                    class="v-progress-linear__bar"
                                                >
                                                    <div
                                                        class="v-progress-linear__bar__indeterminate v-progress-linear__bar__indeterminate--active"
                                                    >
                                                        <div
                                                            class="v-progress-linear__bar__indeterminate long primary"
                                                        ></div>
                                                        <div
                                                            class="v-progress-linear__bar__indeterminate short primary"
                                                        ></div>
                                                    </div>
                                                </div>
                                            </div>
                                        </th>
                                    </tr>
                                </thead>
                                <tbody>
                                    <tr>
                                        <td>20221004315</td>
                                        <td>30198</td>
                                        <td style="color: red">8</td>
                                        <td>
                                            <span
                                                class="red"
                                                style="
                                                    background: rgb(
                                                        244,
                                                        67,
                                                        54
                                                    );
                                                "
                                            ></span>
                                        </td>
                                    </tr>
                                    <tr>
                                        <td>20221004314</td>
                                        <td>30181</td>
                                        <td style="color: green">1</td>
                                        <td>
                                            <span
                                                class="red"
                                                style="
                                                    background: rgb(
                                                        76,
                                                        175,
                                                        80
                                                    );
                                                "
                                            ></span>
                                        </td>
                                    </tr>
                                    <tr>
                                        <td>20221004313</td>
                                        <td>30157</td>
                                        <td style="color: green">7</td>
                                        <td>
                                            <span
                                                class="red"
                                                style="
                                                    background: rgb(
                                                        76,
                                                        175,
                                                        80
                                                    );
                                                "
                                            ></span>
                                        </td>
                                    </tr>
                                    <tr>
                                        <td>20221004312</td>
                                        <td>30159</td>
                                        <td style="color: green">9</td>
                                        <td>
                                            <span
                                                class="red"
                                                style="
                                                    background: rgb(
                                                        76,
                                                        175,
                                                        80
                                                    );
                                                "
                                            ></span>
                                        </td>
                                    </tr>
                                    <tr>
                                        <td>20221004311</td>
                                        <td>30136</td>
                                        <td style="color: red">6</td>
                                        <td>
                                            <span
                                                class="red"
                                                style="
                                                    background: rgb(
                                                        244,
                                                        67,
                                                        54
                                                    );
                                                "
                                            ></span>
                                        </td>
                                    </tr>
                                    <tr>
                                        <td>20221004310</td>
                                        <td>30119</td>
                                        <td style="color: green">9</td>
                                        <td>
                                            <span
                                                class="red"
                                                style="
                                                    background: rgb(
                                                        76,
                                                        175,
                                                        80
                                                    );
                                                "
                                            ></span>
                                        </td>
                                    </tr>
                                    <tr>
                                        <td>20221004309</td>
                                        <td>30118</td>
                                        <td style="color: red">8</td>
                                        <td>
                                            <span
                                                class="red"
                                                style="
                                                    background: rgb(
                                                        244,
                                                        67,
                                                        54
                                                    );
                                                "
                                            ></span>
                                        </td>
                                    </tr>
                                    <tr>
                                        <td>20221004308</td>
                                        <td>30132</td>
                                        <td style="color: red">2</td>
                                        <td>
                                            <span
                                                class="red"
                                                style="
                                                    background: rgb(
                                                        244,
                                                        67,
                                                        54
                                                    );
                                                "
                                            ></span>
                                        </td>
                                    </tr>
                                    <tr>
                                        <td>20221004307</td>
                                        <td>30114</td>
                                        <td style="color: red">4</td>
                                        <td>
                                            <span
                                                class="red"
                                                style="
                                                    background: rgb(
                                                        244,
                                                        67,
                                                        54
                                                    );
                                                "
                                            ></span>
                                        </td>
                                    </tr>
                                    <tr>
                                        <td>20221004306</td>
                                        <td>30101</td>
                                        <td style="color: green">1</td>
                                        <td>
                                            <span
                                                class="red"
                                                style="
                                                    background: rgb(
                                                        76,
                                                        175,
                                                        80
                                                    );
                                                "
                                            ></span>
                                        </td>
                                    </tr>
                                </tbody>
                            </table>
                        </div>
                        <div class="pagination">
                            <ul class="page_box">
                                <li class="page">
                                    <span>1-10</span>
                                    of 2581
                                </li>
                                <li class="page_btn">
                                    <i class="van-icon van-icon-arrow-left"
                                        ><!----></i
                                    ><i class="van-icon van-icon-arrow"
                                        ><!----></i
                                    >
                                </li>
                            </ul>
                        </div>
                    </div>
                </div>
                <div class="content" v-if="tabOpen === 2">
                    <div class="content_con">
                        <div class="content_title">
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
                            <p>Emerd Record</p>
                        </div>
                        <div class="parity">
                            <table>
                                <thead>
                                    <tr>
                                        <th>Period</th>
                                        <th>Price</th>
                                        <th>Number</th>
                                        <th>Result</th>
                                    </tr>
                                    <tr
                                        style="
                                            border: 0px;
                                            width: 100%;
                                            display: none;
                                        "
                                    >
                                        <th
                                            colspan="4"
                                            style="height: 0px; line-height: 0"
                                        >
                                            <div class="table_loading">
                                                <div
                                                    class="v-progress-linear__bar"
                                                >
                                                    <div
                                                        class="v-progress-linear__bar__indeterminate v-progress-linear__bar__indeterminate--active"
                                                    >
                                                        <div
                                                            class="v-progress-linear__bar__indeterminate long primary"
                                                        ></div>
                                                        <div
                                                            class="v-progress-linear__bar__indeterminate short primary"
                                                        ></div>
                                                    </div>
                                                </div>
                                            </div>
                                        </th>
                                    </tr>
                                </thead>
                                <tbody>
                                    <tr>
                                        <td>20221004315</td>
                                        <td>30198</td>
                                        <td style="color: red">8</td>
                                        <td>
                                            <span
                                                class="red"
                                                style="background: red"
                                            ></span>
                                        </td>
                                    </tr>
                                    <tr>
                                        <td>20221004314</td>
                                        <td>30181</td>
                                        <td style="color: green">1</td>
                                        <td>
                                            <span
                                                class="red"
                                                style="background: green"
                                            ></span>
                                        </td>
                                    </tr>
                                    <tr>
                                        <td>20221004313</td>
                                        <td>30157</td>
                                        <td style="color: green">7</td>
                                        <td>
                                            <span
                                                class="red"
                                                style="background: green"
                                            ></span>
                                        </td>
                                    </tr>
                                    <tr>
                                        <td>20221004312</td>
                                        <td>30159</td>
                                        <td style="color: green">9</td>
                                        <td>
                                            <span
                                                class="red"
                                                style="background: green"
                                            ></span>
                                        </td>
                                    </tr>
                                    <tr>
                                        <td>20221004311</td>
                                        <td>30136</td>
                                        <td style="color: red">6</td>
                                        <td>
                                            <span
                                                class="red"
                                                style="background: red"
                                            ></span>
                                        </td>
                                    </tr>
                                    <tr>
                                        <td>20221004310</td>
                                        <td>30119</td>
                                        <td style="color: green">9</td>
                                        <td>
                                            <span
                                                class="red"
                                                style="background: green"
                                            ></span>
                                        </td>
                                    </tr>
                                    <tr>
                                        <td>20221004309</td>
                                        <td>30118</td>
                                        <td style="color: red">8</td>
                                        <td>
                                            <span
                                                class="red"
                                                style="background: red"
                                            ></span>
                                        </td>
                                    </tr>
                                    <tr>
                                        <td>20221004308</td>
                                        <td>30132</td>
                                        <td style="color: red">2</td>
                                        <td>
                                            <span
                                                class="red"
                                                style="background: red"
                                            ></span>
                                        </td>
                                    </tr>
                                    <tr>
                                        <td>20221004307</td>
                                        <td>30114</td>
                                        <td style="color: red">4</td>
                                        <td>
                                            <span
                                                class="red"
                                                style="background: red"
                                            ></span>
                                        </td>
                                    </tr>
                                    <tr>
                                        <td>20221004306</td>
                                        <td>30101</td>
                                        <td style="color: green">1</td>
                                        <td>
                                            <span
                                                class="red"
                                                style="background: green"
                                            ></span>
                                        </td>
                                    </tr>
                                </tbody>
                            </table>
                        </div>
                        <div class="pagination">
                            <ul class="page_box">
                                <li class="page">
                                    <span>1-10</span>
                                    of 2581
                                </li>
                                <li class="page_btn">
                                    <i class="van-icon van-icon-arrow-left"
                                        ><!----></i
                                    ><i class="van-icon van-icon-arrow"
                                        ><!----></i
                                    >
                                </li>
                            </ul>
                        </div>
                    </div>
                </div>
                <div class="content_con">
                    <div class="content_title">
                        <svg
                            xmlns="http://www.w3.org/2000/svg"
                            width="49.005"
                            height="60"
                            viewBox="0 0 49.005 60"
                        >
                            <g id="records" transform="translate(-46.914 0)">
                                <path
                                    id="Path_1"
                                    data-name="Path 1"
                                    d="M61.694,24.613H71.832V14.781Z"
                                    transform="translate(-13.026 -13.027)"
                                    fill="#f4b2b0"
                                />
                                <path
                                    id="Path_2"
                                    data-name="Path 2"
                                    d="M58.806,13.34H48.668a1.754,1.754,0,0,1-1.221-3.013L57.585.495A1.754,1.754,0,0,1,60.56,1.754v9.832A1.754,1.754,0,0,1,58.806,13.34ZM53,9.832h4.056V5.9Z"
                                    fill="#b3404a"
                                />
                                <path
                                    id="Path_3"
                                    data-name="Path 3"
                                    d="M230.482,37.974a1.754,1.754,0,0,1-1.754-1.754V4.289a.823.823,0,0,0-.859-.78H202.633a1.754,1.754,0,0,1,0-3.508h25.236a4.333,4.333,0,0,1,4.367,4.288v31.93A1.754,1.754,0,0,1,230.482,37.974Z"
                                    transform="translate(-136.317 -0.001)"
                                    fill="#b3404a"
                                />
                                <path
                                    id="Path_4"
                                    data-name="Path 4"
                                    d="M91.608,60H51.228a4.278,4.278,0,0,1-4.312-4.234V11.441a1.732,1.732,0,0,1,.526-1.243L57.452.489a1.732,1.732,0,1,1,2.411,2.486l-9.484,9.2V55.766a.813.813,0,0,0,.848.77H91.608a.813.813,0,0,0,.848-.77V44.907a1.732,1.732,0,1,1,3.464,0V55.766A4.278,4.278,0,0,1,91.608,60Z"
                                    transform="translate(-0.002 -0.001)"
                                    fill="#b3404a"
                                />
                                <path
                                    id="Path_5"
                                    data-name="Path 5"
                                    d="M230.481,13.342H202.632a1.754,1.754,0,1,1,0-3.508h26.095v-5.1a1.223,1.223,0,0,0-1.222-1.222H202.632a1.754,1.754,0,1,1,0-3.508h24.873a4.735,4.735,0,0,1,4.73,4.73v6.857A1.754,1.754,0,0,1,230.481,13.342Z"
                                    transform="translate(-136.316 -0.002)"
                                    fill="#b3404a"
                                />
                                <rect
                                    id="Rectangle_1"
                                    data-name="Rectangle 1"
                                    width="14.733"
                                    height="7.717"
                                    transform="translate(55.421 22.174)"
                                    fill="#f4b2b0"
                                />
                                <rect
                                    id="Rectangle_2"
                                    data-name="Rectangle 2"
                                    width="14.733"
                                    height="7.717"
                                    transform="translate(55.421 40.489)"
                                    fill="#f4b2b0"
                                />
                                <path
                                    id="Path_6"
                                    data-name="Path 6"
                                    d="M121.609,186.009H106.875a1.754,1.754,0,0,1-1.754-1.754v-7.717a1.754,1.754,0,0,1,1.754-1.754h14.734a1.754,1.754,0,0,1,1.754,1.754v7.717A1.754,1.754,0,0,1,121.609,186.009Zm-12.98-3.508h11.226v-4.209H108.629Z"
                                    transform="translate(-51.299 -154.361)"
                                    fill="#b3404a"
                                />
                                <path
                                    id="Path_7"
                                    data-name="Path 7"
                                    d="M301.807,189.286h0a1.754,1.754,0,0,1-1.24-.514l-2.806-2.806a1.754,1.754,0,1,1,2.481-2.48l1.566,1.566,5.457-5.457a1.754,1.754,0,0,1,2.481,2.48l-6.7,6.7A1.755,1.755,0,0,1,301.807,189.286Z"
                                    transform="translate(-221.248 -158.148)"
                                    fill="#b3404a"
                                />
                                <path
                                    id="Path_8"
                                    data-name="Path 8"
                                    d="M121.609,342.6H106.875a1.754,1.754,0,0,1-1.754-1.754v-7.717a1.754,1.754,0,0,1,1.754-1.754h14.734a1.754,1.754,0,0,1,1.754,1.754v7.717A1.754,1.754,0,0,1,121.609,342.6Zm-12.98-3.508h11.226V334.88H108.629Z"
                                    transform="translate(-51.299 -292.652)"
                                    fill="#b3404a"
                                />
                                <path
                                    id="Path_9"
                                    data-name="Path 9"
                                    d="M301.807,345.875h0a1.754,1.754,0,0,1-1.24-.514l-2.806-2.806a1.754,1.754,0,1,1,2.481-2.48l1.566,1.566,5.457-5.457a1.754,1.754,0,0,1,2.481,2.48l-6.7,6.7A1.756,1.756,0,0,1,301.807,345.875Z"
                                    transform="translate(-221.248 -296.44)"
                                    fill="#b3404a"
                                />
                            </g>
                        </svg>

                        <p>My Record</p>
                    </div>
                    <div class="parity">
                        <p
                            style="
                                font-size: 12px;
                                text-align: center;
                                padding: 15px 0px;
                                color: rgb(136, 136, 136);
                            "
                        >
                            There is no unsettled order at present. If you want
                            to query the settled order, please go to the order
                            record to query
                        </p>
                    </div>
                    <div class="pagination">
                        <ul class="page_box">
                            <li class="page">
                                <span>1-10</span>
                                of 0
                            </li>
                            <li class="page_btn">
                                <i class="van-icon van-icon-arrow-left"
                                    ><!----></i
                                ><i class="van-icon van-icon-arrow"><!----></i>
                            </li>
                        </ul>
                    </div>
                </div>
                <div class="order-btn">
                    <button class="order_btn one_btn">My Orders</button>
                </div>
            </div>

            <div v-if="isShow" class="agree_zz">
                <div class="wrapper">
                    <p
                        class="branch_title"
                        style="background: rgb(76, 175, 80)"
                    >
                        Join Green
                    </p>
                    <div class="branch_content">
                        <p class="money">Contract Money</p>
                        <div class="choose_money">
                            <ul>
                                <li class="active">10</li>
                                <li class="">100</li>
                                <li class="">1000</li>
                                <li class="">10000</li>
                            </ul>
                        </div>
                        <p class="money">Number</p>
                        <div class="stepper">
                            <div class="van-stepper">
                                <button
                                    type="button"
                                    class="van-stepper__minus van-stepper__minus--disabled"
                                ></button
                                ><input
                                    type="text"
                                    role="spinbutton"
                                    inputmode="decimal"
                                    aria-valuemax="Infinity"
                                    aria-valuemin="1"
                                    aria-valuenow="1"
                                    value="1"
                                    class="van-stepper__input"
                                /><button
                                    type="button"
                                    class="van-stepper__plus"
                                ></button>
                            </div>
                        </div>
                        <p class="money">
                            Total contract money is
                            <span>10</span>
                        </p>
                        <div class="agree_box">
                            <div
                                role="checkbox"
                                tabindex="0"
                                aria-checked="true"
                                class="van-checkbox"
                            >
                                <div
                                    class="van-checkbox__icon van-checkbox__icon--square van-checkbox__icon--checked"
                                >
                                    <i
                                        class="van-icon van-icon-success"
                                        style="
                                            border-color: rgb(0, 0, 0);
                                            background-color: rgb(0, 0, 0);
                                        "
                                        ><!----></i
                                    >
                                </div>
                                <span class="van-checkbox__label"
                                    >I agree
                                    <span class="greencolor"
                                        >PRESALE RULE</span
                                    ></span
                                >
                            </div>
                        </div>
                        <div class="close_btn">
                            <button @click="isShow = !isShow">CANCEL</button
                            ><button
                                @click="isShow = !isShow"
                                style="color: rgb(0, 137, 123)"
                            >
                                CONFIRM
                            </button>
                        </div>
                    </div>
                </div>
            </div>
        </section>
    </main>
</template>

<script>
import HeaderItem from "../components/HeaderItem.vue";
export default {
    name: "DashboardView",
    components: {
        HeaderItem,
    },
    data() {
        return {
            tabOpen: 1,
            isShow: false,
        };
    },
    methods: {
        tab(value) {
            this.tabOpen = value;
        },
        activeLink() {
            this.isActive = !this.isActive; // Toggle Class
        },
    },
};
</script>

<style scoped>
.main_nav {
    width: 100%;
    display: flex;
    flex-direction: row;
    justify-content: space-between;
}
.main_nav li {
    flex: 1;
    font-size: 14px;
    height: 48px;
    line-height: 48px;
    text-align: center;
    opacity: 0.7;
    cursor: pointer;
}
.main_nav li.active {
    opacity: 1;
    border-bottom: 2px solid #f81f01;
    color: #f81f01;
}
.center_text {
    width: 100%;
    padding: 15px 0 5px;
    background: #fafafa;
}
.center_top {
    width: 100%;
    padding: 0 15px;
    box-sizing: border-box;
    display: flex;
    flex-direction: row;
}
.center_top li {
    width: 50%;
}

.nav_content {
    background-color: #ddd;
}
.center_top li .top_ol {
    display: flex;
    flex-direction: row;
    align-items: center;
    font-size: 18px;
    color: #7d7d7d;
}
.center_top li .top_ol svg {
    width: 20px;
    height: 20px;
    margin-right: 10px;
}
.bot_ol {
    margin-top: 12px;
    font-size: 22px;
    color: rgba(0, 0, 0, 0.87);
}
.right_li {
    display: flex;
    flex-direction: column;
    align-items: flex-end;
    justify-content: flex-end;
}
.bot_ol {
    margin-top: 12px;
    font-size: 22px;
    color: rgba(0, 0, 0, 0.87);
}
.van-count-down {
    color: #323233;
    font-size: 14px;
    line-height: 20px;
}
.bot_ol .countdown .van-count-down {
    display: flex;
    flex-direction: row;
    align-items: center;
}
.bot_ol .countdown .van-count-down {
    display: flex;
    flex-direction: row;
    align-items: center;
    display: inline-block;
    padding: 5px 5px;
    border-radius: 5px;
    background: #f2f2f2;
}
.bot_ol .countdown .span {
    display: inline-block;
    padding: 5px 5px;
    border-radius: 5px;
    background: #f2f2f2;
}
.grayback {
    background: #dcdcdc !important;
    color: #333 !important;
}
.bot_ol .ol_btn button {
    padding: 10px 16px;
    font-size: 14px;
    border-radius: 2px;
    border: 0;
    background: #ff9800;
    color: #fff;
}
.btn_center {
    width: 100%;
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: space-between;
    padding: 10px 15px 15px;
    box-sizing: border-box;
    margin-top: 12px;
}
.back_one {
    background: #4caf50;
    color: #fff;
}
.back_two {
    background: #9c27b0;
    color: #fff;
}
.back_three {
    background: linear-gradient(145deg, #f81f01, #ee076e);
    color: #fff;
}
.btn_center button {
    cursor: pointer;
    padding: 10px 16px;
    font-size: 14px;
    border-radius: 2px;
    border: 0;
    box-shadow: 0 3px 1px -2px rgba(0, 0, 0, 0.2),
        0 2px 2px 0 rgba(0, 0, 0, 0.14), 0 1px 5px 0 rgba(0, 0, 0, 0.12);
    transition: 0.3s cubic-bezier(0.25, 0.8, 0.5, 1), color 1ms;
}
.bot_ol .countdown .van-count-down {
    display: flex;
    flex-direction: row;
    align-items: center;
}
.bot_ol .countdown span {
    color: #0f1223;
    margin-left: 5px;
    font-size: 24px;
}
.center_notes {
    display: flex;
    flex-direction: row;
    flex-wrap: wrap;
    padding: 0 7.5px;
    box-sizing: border-box;
}
.center_notes li {
    width: 20%;
    padding: 0 7.5px;
    display: flex;
    justify-content: center;
    cursor: pointer;
}
.center_notes li ol {
    display: inline-block;
    padding: 10px 0;
    text-align: center;
    font-size: 14px;
    width: 100%;
    color: #fff;
    border-radius: 2px;
    background: #2196f3;
    margin-bottom: 15px;
    box-shadow: 0 3px 1px -2px rgba(0, 0, 0, 0.2),
        0 2px 2px 0 rgba(0, 0, 0, 0.14), 0 1px 5px 0 rgba(0, 0, 0, 0.12);
    transition: 0.3s cubic-bezier(0.25, 0.8, 0.5, 1), color 1ms;
}
.content {
    background: #fafafa;
}
.content_con {
    box-shadow: 0 0 0 0 rgba(0, 0, 0, 0.2), 0 0 0 0 rgba(0, 0, 0, 0.14),
        0 0 0 0 rgba(0, 0, 0, 0.12);
    transition: 0.3s cubic-bezier(0.25, 0.8, 0.5, 1);
    background: #fff;
    border-bottom: 1px solid #a6a6a6;
    margin-bottom: 15px;
    border-radius: 3px;
}
.content_title {
    width: 100%;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    border-bottom: 2px solid #009587;
    padding: 12px 0;
}
.content_title svg {
    width: 20px;
    height: 20px;
}
.content_title p {
    color: rgba(0, 0, 0, 0.87);
    font-size: 14px;
    margin-top: 10px;
}
.parity {
    width: 100%;
}
.parity table {
    width: 100%;
    border-collapse: collapse;
}
.parity table tr {
    border-bottom: 1px solid #e0e0e0;
}
.parity table th {
    width: 20%;
    height: 56px;
    line-height: 56px;
    color: rgba(0, 0, 0, 0.54);
    font-size: 12px;
    text-align: center;
}
.parity table td {
    height: 48px;
    line-height: 48px;
    font-size: 12px;
    text-align: center;
}
.parity table tr td span {
    width: 15px;
    height: 15px;
    display: inline-block;
    border-radius: 50%;
    margin: 0 2px;
}
.red {
    background: #f44336;
}
.pagination {
    height: 50px;
    line-height: 50px;
    display: flex;
    justify-content: flex-end;
    align-items: flex-end;
    padding: 0 15px;
    box-sizing: border-box;
}
.pagination .page_box {
    width: 50%;
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: space-between;
}
.pagination .page_box .page {
    font-size: 12px;
    color: rgba(0, 0, 0, 0.54);
}
.one_btn {
    background: #2196f3 !important;
    color: #fff !important;
}
.order_btn {
    padding: 0 15px;
    box-shadow: 0 3px 1px -2px rgb(0 0 0/20%), 0 2px 2px 0 rgb(0 0 0/14%),
        0 1px 5px 0 rgb(0 0 0/12%);
    color: rgba(0, 0, 0, 0.87);
    height: 36px;
    line-height: 36px;
    font-size: 14px;
    border: 0;
    border-radius: 2px;
    background: #f5f5f5;
    margin-right: 10px;
    cursor: pointer;
}
.order-btn {
    text-align: center;
    padding: 20px 0;
}
.agree_zz {
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background: rgba(0, 0, 0, 0.4);
    display: flex;
    justify-content: center;
    align-items: center;
    z-index: 99;
}
.wrapper {
    background: #fff;
    border-radius: 4px;
    width: 90%;
    box-shadow: 0 3px 1px -2px rgba(0, 0, 0, 0.2),
        0 2px 2px 0 rgba(0, 0, 0, 0.14), 0 1px 5px 0 rgba(0, 0, 0, 0.12);
    transition: 0.3s cubic-bezier(0.25, 0.8, 0.5, 1);
    overflow: hidden;
    position: relative;
}
.branch_title {
    padding: 15px;
    box-sizing: border-box;
    font-size: 24px;
    color: #fff;
}
.branch_content {
    padding: 15px 30px 50px 30px;
    box-sizing: border-box;
}
.money {
    margin-bottom: 15px;
    font-size: 14px;
    color: #212121;
}
.choose_money {
    margin-bottom: 15px;
    display: flex;
}
.choose_money ul {
    display: flex;
    flex-direction: row;
    align-items: center;
    box-shadow: 0 3px 1px -2px rgba(0, 0, 0, 0.2),
        0 2px 2px 0 rgba(0, 0, 0, 0.14), 0 1px 5px 0 rgba(0, 0, 0, 0.12);
    transition: 0.3s cubic-bezier(0.25, 0.8, 0.5, 1);
    border-radius: 2px;
    overflow: hidden;
    justify-content: space-between;
}
.choose_money ul li {
    padding: 10px 10px;
    font-size: 14px;
    color: #a6a6a6;
    cursor: pointer;
}
.choose_money ul .active {
    background: #c9c9c9;
    color: #333;
}
.stepper {
    margin-bottom: 40px;
}
.van-stepper {
    font-size: 0;
    -webkit-user-select: none;
    user-select: none;
}
.stepper .van-stepper {
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    align-items: center;
}

.van-stepper__minus,
.van-stepper__plus {
    position: relative;
    box-sizing: border-box;
    width: 28px;
    height: 28px;
    margin: 0;
    padding: 0;
    color: #323233;
    vertical-align: middle;
    background-color: #f2f3f5;
    border: 0;
    cursor: pointer;
}
.van-stepper__minus--disabled,
.van-stepper__plus--disabled {
    color: #c8c9cc;
    background-color: #f7f8fa;
    cursor: not-allowed;
}
.van-stepper__minus {
    border-radius: 4px 0 0 4px;
}
.stepper .van-stepper button {
    width: 56px;
    height: 36px;
    display: flex;
    justify-content: center;
    align-items: center;
    box-shadow: 0 3px 1px -2px rgba(0, 0, 0, 0.2),
        0 2px 2px 0 rgba(0, 0, 0, 0.14), 0 1px 5px 0 rgba(0, 0, 0, 0.12);
    background: #f5f5f5;
    transition: 0.3s cubic-bezier(0.25, 0.8, 0.5, 1), color 1ms;
}
.van-stepper__input {
    box-sizing: border-box;
    width: 32px;
    height: 28px;
    margin: 0 2px;
    padding: 0;
    color: #323233;
    font-size: 14px;
    line-height: normal;
    text-align: center;
    vertical-align: middle;
    background-color: #f2f3f5;
    border: 0;
    border-width: 1px 0;
    border-radius: 0;
    appearance: none;
    -webkit-appearance: none;
}
.stepper .van-stepper input {
    background: transparent;
    font-size: 24px;
}
.close_btn {
    height: 48px;
    position: absolute;
    bottom: 0;
    left: 0;
    width: 100%;
    display: flex;
    justify-content: flex-end;
    padding: 0 15px;
    box-sizing: border-box;
    background: #fff;
}
.close_btn button {
    border: 0;
    background: transparent;
    font-size: 14px;
    color: rgba(0, 0, 0, 0.9);
    margin: 0 10px 0 20px;
    cursor: pointer;
}
.agree_box .greencolor {
    color: #009688;
    font-weight: 400;
    cursor: pointer;
}
.van-stepper__minus:after,
.van-stepper__minus:before,
.van-stepper__plus:after,
.van-stepper__plus:before {
    position: absolute;
    top: 50%;
    left: 50%;
    background-color: currentColor;
    -webkit-transform: translate(-50%, -50%);
    transform: translate(-50%, -50%);
    content: "";
}
.stepper .van-stepper .van-stepper__minus:before,
.stepper .van-stepper .van-stepper__plus:before {
    width: 34%;
    height: 1px;
    color: #000;
}
.van-stepper__minus:after,
.van-stepper__plus:after {
    width: 1px;
    height: 50%;
}
.van-stepper__minus:after {
    display: none;
}
</style>
