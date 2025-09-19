print("Your Favorite Movies.")

favorite_movies_list = []

add_movie = input("Input your favorite movies: ")

if add_movie.lower() != "none":
    favorite_movies_list = [movie.strip() for movie in add_movie.split(",")]

remove_movie = input("Is there a movie you would like to remove from favorites (or type none): ")

if remove_movie.lower() != "none":
    if remove_movie in favorite_movies_list:
        favorite_movies_list.remove(remove_movie)
    else:
        print(f"'{remove_movie}' not found in favorites!")

favorite_movies_list.sort()

print(f"Your Favorite Movies are: {favorite_movies_list}")

