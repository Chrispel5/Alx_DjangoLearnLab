# Retrieve the Book

from bookshelf.models import Book
book = Book.objects.get(title="1984")
{field.name: getattr(book, field.name) for field in book._meta.fields}

# Output: {'id': 1, 'title': '1984', 'author': 'George Orwell', 'publication_year': 1949}
