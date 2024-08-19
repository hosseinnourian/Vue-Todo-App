<template>
    <div class="assistance-holder">
        <div class="search-bar">
            <input class="search-input" placeholder="Search Note..." type="text">
        </div>
        <div class="sort-bar">
            <select class="sort-select" name="" id="">
                <option value="">All</option>
                <option value="">Completed</option>
                <option value="">In Progress</option>
            </select>
        </div>
        <div class="night-mode">
            <button class="night-mode-btn">
                <img src="../assets/m.png" alt="#">
            </button>
        </div>
    </div>
</template>


<style scoped>
.assistance-holder {
    margin: 40px auto;
    width: 80%;
    display: flex;
    padding: 20px 0;
}
.search-bar {
    flex-grow: 3;
}
.search-input {
    width: 100%;
    padding: 15px 5px;
    border-radius: 8px;
    border: 3px solid rgb(105, 126, 228);
    font-size: 20px;
}
.sort-bar {
    flex-grow: 1;
    display: flex;
    align-items: center;
    justify-content: center;
}
.sort-select{
    background-color: rgb(105, 126, 228);
    color: white;
    padding: 15px 20px;
    font-size: 20px;
    font-weight: bold;
    border-radius: 8px;
}
.night-mode {
    border-radius: 8px;
    background-color: rgb(105, 126, 228);
    flex-grow: 0;
   flex-shrink: 0;
   flex-basis: 7%;
}
.night-mode > .night-mode-btn{
    background : none;
   display: block;
   margin: 5px auto;
   border: none;
}
.night-mode > .night-mode-btn img {
    width: 40px;
    height: 40px;
}
</style>