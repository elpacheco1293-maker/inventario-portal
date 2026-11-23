# Portal de Inventarios · Nexocorp (Supabase + GitHub + Vercel)

1. **Supabase**: SQL Editor → pega y ejecuta `supabase/schema.sql`, y luego `supabase/usuarios.sql`.
   Authentication → Sign In / Providers → Email: desactiva *Allow new users to sign up*.
2. **config.js**: pon tu Project URL y la anon public key.
3. **GitHub**: sube la carpeta a un repo. **Vercel**: Import Project (sin variables, sin build).

Ingreso: admin / 123456 · bodegas: B301 / B301, B302 / B302, …
Cambia las claves desde Admin → Claves.

Eliminar una solicitud (botón en su detalle) borra en cascada todo lo asociado.
Para que el disco baje: `vacuum full public.counts; vacuum full public.articles;`
