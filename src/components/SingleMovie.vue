<template>
    <div :class="movie.movie_released ? 'yes' :'no' ">
        <h1>{{movie.movie_name}}</h1>
        
            <h2 class="flex">Year: {{movie.movie_year}}</h2>
        
        <h2 class="flex">Runtime: {{movie.movie_runtime}}</h2>
        <h2 class="genre">Genre: {{movie.movie_genre}}</h2>
        <h2 class="language">Language: {{movie.movie_language}}</h2>
        <h2 class="flex">Rating: {{movie.movie_rating}}</h2>
        <h2 class="flex">Director: {{movie.movie_director}}</h2>
        <h2 class="flex">Actors: {{movie.movie_actors}}</h2>
        <h2 class="flex">Released: {{movie.movie_released}}</h2>
    </div>
</template>
<script>
export default{
    name: 'SingleMovie',
    props:{
        movie: Array
}
}
</script>
<style scoped>
.yes{
    background-color: #9fe2bf;
}
.no{
    background-color: #e2bf9f;
}
div{
    color: black;
    padding: 1em;
    text-align: center;
    margin: 1em;
    width: 75%;
    margin-left:10%;
    border: 1px solid #234d37;
    border-radius: 10px;
}
h2{
    font-size: 1em;
}
h4{
    margin: 2px;
}
.genre,.language,.flex{
  border:1px solid black;
  padding: 7px;
  border-radius: 10px;
  width:30%;
  margin:5px auto;
}
</style>