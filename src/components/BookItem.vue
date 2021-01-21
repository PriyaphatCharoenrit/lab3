<template>
    <div>
        <div class="book-item"> 
            <h1>{{book.title}}</h1><br/>

            <div style="width:100%;text-align:left;">
                <img style="float: left;padding:20px" width="200px" v-bind:src="book.thumbnailUrl" /><br/>
                <div style="oadding:20px">
                    <b>Author:</b>{{book.author}}<br/>
                    <b>Category:</b>{{book.category}}<br/>
                    <b>ISBN:</b>{{book.isbn}}<br/>
                    <b>Pages:</b>{{book.pageCount}}<br/>
                    <b>Description:</b><br/>
                    <p>{{book.shortDescription}}</p>
                </div>
            </div><br/>
        </div>
    </div>
</template>



<script>
export default {
  name: 'BookItem',
  components: {

  },
  props:["book"]
  
}
</script>



<style>
.book-item{
    width: 70%;
    background: #f4f4f4;
    padding: 10px;
    border-bottom: 1px #ccc dotted;
}
</style>
