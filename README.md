# get_next_line

#Subject
Des appels successifs à votre fonction get_next_line() doivent vous permettre de
lire l’intégralité du fichier texte référencé par le descripteur de fichier, une ligne
à la fois.
• Votre fonction doit retourner la ligne qui vient d’être lue.
S’il n’y a plus rien à lire, ou en cas d’erreur, elle doit retourner NULL.
• Assurez-vous que votre fonction se comporte correctement qu’elle lise un fichier
ou qu’elle lise sur l’entrée standard.
• Important : Vous devez toujours retourner la ligne qui a été lue suivie du \n la
terminant, sauf dans le cas où vous avez atteint la fin du fichier et que ce dernier
ne se termine pas par un \n.
• Le fichier d’en-tête get_next_line.h doit contenir au minimum le prototype de
la fonction.
• Le fichier get_next_line_utils.c vous servira à ajouter des fonctions supplé-
mentaires nécessaires à la réalisation de votre get_next_line().

# Fuctions :
  #get_next-line.c
    - *get_next_line(int fd)
    - read_and_stash(int fd, t_list **stash)
    - add_to_stash(t_list **stash, char *buf, int readed)
    - extract_line(t_list *stash, char **line)
    - clean_stash(t_list **stash)

  #get_next_line_utils.c
    - found_newline(t_list *stash)
    - *ft_lst_get_last(t_list *stash)
    - generate_line(char **line, t_list *stash)
    - free_stash(t_list *stash)
    - ft_strlen(const char *str)
