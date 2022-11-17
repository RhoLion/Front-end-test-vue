          <template>
            <div>
              <Navigation/>
              <LearnCoding/>
              <BrowseCategory/>
              <Articles/>
              <Subscribe/>
              <FooterComponent/>
            </div>
          </template>

          <script>
          import Navigation from "@/components/Navigation";
          import LearnCoding from "@/components/LearnCoding";
          import BrowseCategory from "@/components/BrowseCategory";
          import Articles from "@/components/Articles";
          import Subscribe from "@/components/Subscribe";
          import FooterComponent from "@/components/FooterComponent";
          export default {
            name:'theHome',
            components: {
              Navigation,
              LearnCoding,
              BrowseCategory,
              Articles,
              Subscribe,
              FooterComponent
            }
          }
          </script>