<template>
    <div class="row">
        <div class="container">

            <div class="card mt-4 col-sm-6 col-12 mx-auto">
                <div class="card-header text-center"><h3>API - Library</h3></div>
                <div class="card-body">
                        <h5 class="text-dark">Get all books: </h5>
                        <p class="bg-secondary "><i>{{ url }}</i> books</p>
                        <p><b>Method:</b> GET</p>
                        <b>Successful response: </b>
                        <img :src="urlImage+'books.png'" >
                    <hr>
                        <h5 class="text-dark">Show a specific book: </h5>
                        <p class="bg-secondary"><i>{{ url }}</i> id/edit</p>
                        <p><b>Method:</b> GET, Takes a parameter <b>ID</b></p>
                        <b>Successful response: </b>
                        <img :src="urlImage+'showBook.png'">
                    <hr>
                        <h5 class="text-dark">Store a new book: </h5>
                        <p class="bg-secondary"><i>{{ url }}</i> books</p>
                        <p><b>Method:</b> POST</p>
                    <hr>
                        <h5 class="text-dark">Update a specific book: </h5>
                        <p class="bg-secondary"><i>{{ url }}</i> book/id/</p>
                        <p><b>Method:</b> PUT, Takes a parameter <b>ID</b></p>
                        <b>Successful response: </b>
                        <img :src="urlImage+'updateBook.png'">
                    <hr> <!-- NEW DOCUMENTATION -->
                        <h5 class="text-dark">Delete a specific book: </h5>
                        <p class="bg-secondary"><i>{{ url }}</i> book/id</p>
                        <p><b>Method:</b> DELETE, Takes a parameter <b>ID</b></p>
                        <b>Successful response: </b>
                        <img :src="urlImage+'deleteBook.png'">
                    <hr>
                        <h5 class="text-dark">Get total books: </h5>
                        <p class="bg-secondary"><i>{{ url }}</i> totalBooks</p>
                        <p><b>Method:</b> GET</p>
                        <b>Successful response: </b>
                        <img :src="urlImage+'totalBooks.png'">
                </div>
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        name: "ApiMain",
        data: function() {
            return {
                url: 'http://localhost/v8_vue_geeklibrary/public/api/',
                urlImage: '../storage/app/public/api/',
            }
        }
    }
</script>

<style scoped>

</style>