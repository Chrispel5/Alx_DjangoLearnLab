# Delete the Book

 book = Book.objects.all()
 book.delete()
# Output: (1, {'bookshelf.Book': 1})

 book = Book.objects.all()
 book 
# Output: <QuerySet []>