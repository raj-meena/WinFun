<template>
    <header>
        <div class="header-main">
            <p class="balance">Available balance: ₹ 0.78</p>
            <div class="mine_info_btn">
                <div class="btn">
                    <button class="one_btn">Recharge</button
                    ><button>Trend</button>
                </div>
                <div class="refresh">
                    <a href="javascript:void(0)">
                        <svg
                            xmlns="http://www.w3.org/2000/svg"
                            xmlns:xlink="http://www.w3.org/1999/xlink"
                            width="30.004"
                            height="36"
                            viewBox="0 0 30.004 36"
                        >
                            <defs>
                                <linearGradient
                                    id="linear-gradient"
                                    x1="0.5"
                                    x2="0.5"
                                    y2="1"
                                    gradientUnits="objectBoundingBox"
                                >
                                    <stop offset="0" stop-color="#f81f01" />
                                    <stop offset="1" stop-color="#ee076e" />
                                </linearGradient>
                            </defs>
                            <g id="refresh" transform="translate(-0.997)">
                                <path
                                    id="Path_17"
                                    data-name="Path 17"
                                    d="M7.518,17.936A8.576,8.576,0,0,0,16,26.606V28.94l-.944,4.286A15.186,15.186,0,0,1,1,17.936,14.953,14.953,0,0,1,13,3h2l.048,6.323A8.6,8.6,0,0,0,7.518,17.936Z"
                                    fill="#fff"
                                    fill-rule="evenodd"
                                />
                                <path
                                    id="Path_18"
                                    data-name="Path 18"
                                    d="M16,33.275c-.319,0-.63-.029-.944-.049L16,28.94V26.606a8.672,8.672,0,0,0,0-17.34,8.345,8.345,0,0,0-.949.058L15,7s-.658-4.4,1-4.4A15.172,15.172,0,0,1,31,17.936,15.172,15.172,0,0,1,16,33.275Z"
                                    fill-rule="evenodd"
                                    fill="url(#linear-gradient)"
                                />
                                <path
                                    id="Path_19"
                                    data-name="Path 19"
                                    d="M18,36V22l-7,7Z"
                                    fill="#ee076e"
                                    fill-rule="evenodd"
                                />
                                <path
                                    id="Path_20"
                                    data-name="Path 20"
                                    d="M13.989,0V13l6.024-6.494Z"
                                    fill="#fff"
                                    fill-rule="evenodd"
                                />
                            </g>
                        </svg>
                    </a>
                </div>
            </div>
        </div>
    </header>
</template>

<script>
export default {
    name: "HeaderItem",
};
</script>

<style scoped>
.balance {
    padding: 0 0 10px 0;
    box-sizing: border-box;
    font-size: 18px;
    color: #fff;
}
.mine_info_btn {
    width: 100%;
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    align-items: flex-end;
}
.btn button {
    padding: 0 15px;
    box-shadow: 0 3px 1px -2px rgba(0, 0, 0, 0.2),
        0 2px 2px 0 rgba(0, 0, 0, 0.14), 0 1px 5px 0 rgba(0, 0, 0, 0.12);
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
.btn button.one_btn {
    background: linear-gradient(145deg, #f81f01, #ee076e);
    color: #fff;
}
.refresh svg {
    display: block;
}
</style>
